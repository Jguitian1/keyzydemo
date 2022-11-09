<template>
    <div class="card-carousel">
        <div class="card-img">
            <img :src="currentImage">
            <div class="actions">
                <span @click="prevImage" class="prev">
                    <i class="fas fa-chevron-left"></i>
                </span>
                <span @click="nextImage" class="next">
                    <i class="fas fa-chevron-right"></i>
                </span>
            </div>
        </div>
        <div class="thumbnails">
            <div 
                v-for="(image, index) in  images"
                :key="image.id"
                :class="['thumbnail-image', (activeImage == index) ? 'active' : '']"
                @click="activateImage(index)"
            >
                <img :src="image.thumb">
            </div>
        </div>
    </div>
</template>

<script>

export default {
    data() {
            return {
                //Array to hold all carousel images
                images: [
                    {
                        id: '1',
                        big: "http://localhost:8080/img/castle.b2fb5135.jpg",
                        thumb: 'http://localhost:8080/img/castle.b2fb5135.jpg'
                    },
                    {
                        id: '2',
                        big: 'https://www.planetware.com/wpimages/2020/02/france-in-pictures-beautiful-places-to-photograph-eiffel-tower.jpg',
                        thumb: 'https://www.planetware.com/wpimages/2020/02/france-in-pictures-beautiful-places-to-photograph-eiffel-tower.jpg'
                    },
                    {
                        id: '3',
                        big: 'images/p3.jpeg',
                        thumb: 'images/thumbs/p3.jpeg'
                    },
                    {
                        id: '4',
                        big: 'images/p4.jpeg',
                        thumb: 'images/thumbs/p4.jpeg'
                    }
                ],
                //Index of the active image on the images array
                activeImage: 0
            }
        },
        computed: {
            // currentImage gets called whenever activeImage changes
            // and is the reason why we don't have to worry about the 
            // big image getting updated
            currentImage() {
                return this.images[this.activeImage].big;
            }
        },
        methods: {
            // Go forward on the images array 
            // or go at the first image if you can't go forward :/ 
            nextImage() {
                var active = this.activeImage + 1;
                if(active >= this.images.length) {
                    active = 0;
                }
                this.activateImage(active);
            },
            // Go backwards on the images array 
            // or go at the last image
            prevImage() {
                var active = this.activeImage - 1;
                if(active < 0) {
                    active = this.images.length - 1;
                }
                this.activateImage(active);
            },
            activateImage(imageIndex) {
                this.activeImage = imageIndex;
            }
        }
    }
</script>


<style scoped>
.card-carousel {
    user-select: none;
    position: absolute;
    left: 300px; top: 50px;
    transition-timing-function: ease-in;
    animation: fadeIn .5s;
}
@keyframes fadeIn {
    0% { opacity: 0; }
    100% { opacity: 1; }
  }
.thumbnails {
    display: flex;
    flex-direction: row;
    gap: 10px;
    height: 120px;
}
.thumbnail-image {
    display: flex;
    align-items: center;
    cursor: pointer;
    padding: 2px;
    width: 150px;
    height: 120px;

}
.thumbnail-image > img {
    width: 150px;
    height: 100px;
    transition: all 250ms;
}
.thumbnail-image:hover > img, 
.thumbnail-image.active > img {
    opacity: 0.6;
    box-shadow: 2px 2px 6px 1px rgba(0,0,0, 0.5);
}
.card-img {
    position: relative;
    margin-bottom: 15px;
}
.card-img > img {
    display: block;
    margin: 0 auto;
    width: 800px;
    height: 500px;
}
.actions {
    font-size: 1.5em;
    height: 40px;
    position: absolute;
    top: 50%;
    margin-top: -20px;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    color: #585858;
}
.actions > span {
    cursor: pointer;
    transition: all 250ms;
    font-size: 45px;
}
.actions > span.prev {
    margin-left: 5px;
    background-color: white;
    height: 20px;
    width: 20px;
}
.actions > span.next {
    margin-right: 5px;
    background-color: white;
    height: 20px;
    width: 20px;
}
.actions > span:hover {
    color: #eee;
}
</style>