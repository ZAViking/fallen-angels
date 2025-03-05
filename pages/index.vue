<template>
    <div class="popout-container">
      <div class="popout-content">
        <Nav />

        <section class="hero">
          <div class="hero-content">
            <h1 class="section-heading">Finding Strength in Every Fall</h1>
            <p>Welcome to Fallen Angels, where we embrace life’s challenges and rise stronger together.</p>
            <!-- <div class="hero-buttons">
              <button @click="navigateTo('share-story')">Share Your Story</button>
              <button @click="navigateTo('get-inspired')">Get Inspired</button>
            </div> -->
        </div>
      </section>

      <section class="introduction card">
        <h2>Who We Are</h2>
        <p>
          Fallen Angels is a community built to inspire, support, and guide those facing life’s challenges. Learn more about us and join our mission to make a difference.
        </p>
        <button @click="navigateTo('about-us')">Learn More</button>
      </section>

      <section class="featured-content card">
        <h2>Featured Stories</h2>
        <div class="stories">
          <div v-for="story in featuredStories" :key="story.id" class="story-item">
            <h3>{{ story.title }}</h3>
            <p>{{ story.excerpt }}</p>
            <!-- Use NuxtLink to navigate to the specific story page -->
            <NuxtLink :to="`/Lessons/${story.slug}`" class="read-more-button">Read More</NuxtLink>
          </div>
        </div>
    </section>

      <section class="community-highlights card">
        <h2>Join the Conversation</h2>
        <p>Be part of a supportive community where you can connect, share, and grow together.</p>
        <!-- <div class="button-group">
          <button @click="navigateTo('community')">Explore Community</button>
          <button @click="navigateTo('events')">View Events</button>
        </div> -->
      </section>

      </div>
    </div>
</template>

<script>
  export default {
    name: "HomePage",
    data() {
      return {
        featuredStories: [
          { id: 1, title: "Quotes", slug: "quotes", excerpt: "Some inspirational quotes..." },
          { id: 2, title: "The Let Them Theory", slug: "let-them-theory", excerpt: "Discovering the beauty of being me..." },
        ],
      };
    },
  };
</script>

<style scoped>
.index-page {
  font-family: Arial, sans-serif;
  padding: 30px;
  background-color: white; /* White background for the page */
  color: #333; /* Dark text color */
}

.hero {
  text-align: center;
  padding: 50px;
  background: rgba(255, 255, 255, 0.9); /* Light hero background */
  border-radius: 10px;
  box-shadow: 0px 10px 20px rgba(0, 0, 0, 0.1); /* Light shadow */
}

.hero-buttons button {
  margin: 10px;
  padding: 10px 20px;
  border: none;
  background: #ff6600; /* Orange button color */
  color: white;
  cursor: pointer;
  transition: transform 0.3s;
  border-radius: 5px;
}

.hero-buttons button:hover {
  transform: scale(1.05);
}

.card {
  background: rgba(255, 255, 255, 0.95); /* Slightly opaque background */
  border-radius: 12px;
  padding: 20px;
  margin-top: 20px;
  box-shadow: 0px 5px 15px rgba(0, 0, 0, 0.1);
}

.story-item {
  margin-top: 15px;
  padding: 15px;
  border-radius: 8px;
  background: rgba(255, 255, 255, 0.1);
}

.read-more-button {
  background-color: #ff6600; /* Same orange button color as in the hero section */
  color: white;
  border: none;
  padding: 10px 20px;
  cursor: pointer;
  transition: transform 0.3s;
  border-radius: 5px;
}

.read-more-button:hover {
  transform: scale(1.05);
}

.button-group {
  display: flex;
  gap: 10px;
  justify-content: center;
}

.button-group button {
  padding: 12px 20px;
  background-color: #ff6600; /* Orange button for consistency */
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.button-group button:hover {
  background-color: #cc5200; /* Darker orange on hover */
}
</style>
