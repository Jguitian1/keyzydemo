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
                        big: "https://cdn.cloudflare.steamstatic.com/steam/apps/204360/ss_57cdabd9ae140e33c5551ee0088d1e5db11b4622.1920x1080.jpg?t=1666985972",
                        thumb: 'https://cdn.cloudflare.steamstatic.com/steam/apps/204360/ss_57cdabd9ae140e33c5551ee0088d1e5db11b4622.1920x1080.jpg?t=1666985972'
                    },
                    {
                        id: '2',
                        big: 'https://static.kinguin.net/cdn-cgi/image/w=1140,q=80,fit=scale-down,f=auto/media/category/2/-/2-1024_457.jpg',
                        thumb: 'https://static.kinguin.net/cdn-cgi/image/w=1140,q=80,fit=scale-down,f=auto/media/category/2/-/2-1024_457.jpg'
                    },
                    {
                        id: '3',
                        big: 'https://cdn.akamai.steamstatic.com/steam/apps/204360/ss_9cf7ff6ba267da33e140f66c29f50fd2ed391da2.1920x1080.jpg?t=1666985972',
                        thumb: 'https://cdn.akamai.steamstatic.com/steam/apps/204360/ss_9cf7ff6ba267da33e140f66c29f50fd2ed391da2.1920x1080.jpg?t=1666985972'
                    },
                    {
                        id: '4',
                        big: 'https://cdn.akamai.steamstatic.com/steam/apps/204360/ss_a6a154f004bd7d0c3c7c1a0b378216ce0e8c8dd2.1920x1080.jpg?t=1666985972',
                        thumb: 'https://cdn.akamai.steamstatic.com/steam/apps/204360/ss_a6a154f004bd7d0c3c7c1a0b378216ce0e8c8dd2.1920x1080.jpg?t=1666985972'
                    },
                    {
                        id: '5',
                        big: 'https://cdn.akamai.steamstatic.com/steam/apps/204360/ss_2f53c16cb83d492cae0421ca090d2591f863e448.1920x1080.jpg?t=1666985972',
                        thumb: 'https://cdn.akamai.steamstatic.com/steam/apps/204360/ss_2f53c16cb83d492cae0421ca090d2591f863e448.1920x1080.jpg?t=1666985972'
                    },

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
    gap: 12.5px;
    height: 120px;
}
.thumbnail-image {
    display: flex;
    align-items: center;
    cursor: pointer;
    width: 150px;
    height: 120px;

}
.thumbnail-image > img {
    width: 150px;
    height: 100px;
    transition: all 250ms;
}
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
    height: 70px;
    width: 20px;
}
.actions > span.next {
    margin-right: 5px;
    background-color: white;
    height: 70px;
    width: 20px;
}
.actions > span:hover {
    color: #eee;
}
</style>