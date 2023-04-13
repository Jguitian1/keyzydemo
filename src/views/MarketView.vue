<template>
  <div class="market">
    <h1>Market</h1>
    <div class="market-items">
      <div
        class="market-item"
        v-for="item in items"
        :key="item.id"
      >
        <img :src="item.image" :alt="item.title" class="item-image" />
        <div class="item-info">
          <h3>{{ item.title }}</h3>
          <p>{{ item.price }}</p>
          <button class="item-buy-button">Buy</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
  return {
    items: [
      {
        id: 1,
        title: 'Counter Strike Global Offensive',
        image: 'https://cdn.akamai.steamstatic.com/steam/apps/730/header.jpg?t=1668125812',
        price: '$14.99',
      },
      {
        id: 2,
        title: 'AWP | Dragon Lore',
        image: 'https://cdn.csgoskins.gg/public/uih/products/aHR0cHM6Ly9zdGVhbWNvbW11bml0eS1hLmFrYW1haWhkLm5ldC9lY29ub215L2ltYWdlLy05YTgxZGxXTHdKMlVVR2NWc19uc1Z0emRPRWR0V3dLR1paTFFIVHhEWjdJNTZLVTBad3dvNE5VWDRvRkpaRUhMYlhINUFwZU80WW1saHhZUWtuQ1J2Q28wNERFVmx4a0tncG90NjIxRkFSMTdQN05kVFJILXQyNnE0U1psdkQ3UFlUUWdYdHU1TXgyZ3YzLS1ZM25qMUg2cUJGdk1XSHlJbzdBZHc5cmFGNkdybEs5bExpLWpKTzd0Sl9KenlOaDYzRjNzWF9lbVVQa2dRWU1NTEwyTURSQWJRLzUxMngzODQ-/auto/auto/85/notrim/669993d9d3d2cb915539c081390131a6.webp',
        price: '$1500',
      },
      {
        id: 3,
        title: 'AK-47 | Fire Serpent',
        image: 'https://cdn.csgoskins.gg/public/uih/products/aHR0cHM6Ly9zdGVhbWNvbW11bml0eS1hLmFrYW1haWhkLm5ldC9lY29ub215L2ltYWdlLy05YTgxZGxXTHdKMlVVR2NWc19uc1Z0emRPRWR0V3dLR1paTFFIVHhEWjdJNTZLVTBad3dvNE5VWDRvRkpaRUhMYlhINUFwZU80WW1saHhZUWtuQ1J2Q28wNERFVmx4a0tncG90N0h4ZkRoanhzek9lQzlIXzlta2hJV0ZnOGoxT08tR3FXbEQ2ZE4tdGVYSThvVGh0MWkxdVJRNWZXRHdMWWJBZFZCcVlWSFJyd0Mya083cmhwTHE2Sl9JelhFMnVuRnhzMy1KbWtHMjAwb2ZaLUp4eGF2SktaaU90NGsvNTEyeDM4NA--/auto/auto/85/notrim/3ef2ffaed1a9547f17c53fbb7aff3687.webp',
        price: '$400',
      },
      {
        id: 4,
        title: 'Spectrum Case',
        image: 'https://cdn.csgoskins.gg/public/uih/products/aHR0cHM6Ly9zdGVhbWNvbW11bml0eS1hLmFrYW1haWhkLm5ldC9lY29ub215L2ltYWdlLy05YTgxZGxXTHdKMlVVR2NWc19uc1Z0emRPRWR0V3dLR1paTFFIVHhEWjdJNTZLVTBad3dvNE5VWDRvRkpaRUhMYlhVNUExUElZUU5xaHBPU1YtZlJQYXN3OHJzVUZKNUtCRlp2NjY4RkZZMm5mS2FkRDRVN1k3bHdZWGV4YUdsWWIzUXpqbFV2WjBrMHVqSHB0dWcyVmJpcmtSck5XMm1kNFNMTWxocGgwOWhwWDAvNTEyeDM4NA--/auto/auto/85/notrim/eb2ca02831fd93604adfbf100e9cfb57.webp',
        price: '$2.49',
      },
      {
        id: 5,
        title: 'Chroma Case',
        image: 'https://cdn.csgoskins.gg/public/uih/products/aHR0cHM6Ly9zdGVhbWNvbW11bml0eS1hLmFrYW1haWhkLm5ldC9lY29ub215L2ltYWdlLy05YTgxZGxXTHdKMlVVR2NWc19uc1Z0emRPRWR0V3dLR1paTFFIVHhEWjdJNTZLVTBad3dvNE5VWDRvRkpaRUhMYlhVNUExUElZUU5xaHBPU1YtZlJQYXN3OHJzVUZKNUtCRlp2NjY4RkZFdWhfS1FKVHRFdUk2M3hJWGJ4cU90YXV5Q2xUTUVzSlYxanJ1Uzg5VDNpUUt4X0JCcWEyajNKcGpWTEZIMXhwcDBFUS81MTJ4Mzg0/auto/auto/85/notrim/298d8fb88bfba7e532a26c4a2fdaa56d.webp',
        price: '$1.99',
      },
    ],
  };
},

};
</script>

<style scoped>
.market {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 2rem;
  margin-left: 200px;
}

h1 {
  font-size: 2rem;
  margin-bottom: 1rem;
  color: #4a4a4a;
}

.market-items {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
  justify-content: center;
  max-width: 100%;
  overflow-x: auto;
}

.market-item {
  display: flex;
  flex-direction: column;
  align-items: center;
  background-color: transparent;
  border-radius: 10px;
  padding: 1rem;
  width: 300px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.item-image {
  width: 100%;
  height: auto;
  object-fit: cover;
  border-radius: 5px;
}

.item-info {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 1rem;
}

.item-info h3 {
  font-size: 1.25rem;
  margin-bottom: 0.5rem;
  color: #4a4a4a;
}

.item-info p {
  font-size: 1rem;
  margin-bottom: 1rem;
  color: #4a4a4a;
}

.item-buy-button {
  background-color: #0080ff;
  color: white;
  border: none;
  border-radius: 5px;
  padding: 10px 20px;
  font-size: 1rem;
  cursor: pointer;
  transition: background-color 0.2s ease;
}

.item-buy-button:hover {
  background-color: #0069d9;
}
</style>
