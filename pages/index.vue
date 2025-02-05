<template>
  <div class="Let-Them-Tasks">
    <!-- Hero Section -->
    <section class="hero">
      <div class="hero-content">
        <h1 class="section-heading">Finding Strength in Every Fall</h1>
        <p>Welcome to Fallen Angels, where we embrace life’s challenges and rise stronger together.</p>
        <div class="hero-buttons">
          <button @click="navigateTo('share-story')">Share Your Story</button><br />
          <button @click="navigateTo('get-inspired')">Get Inspired</button>
        </div>
      </div>
    </section>

    <!-- Introduction Section -->
    <section class="introduction">
      <h2 class="sub-heading">Who We Are</h2>
      <p>
        Fallen Angels is a community built to inspire, support, and guide those facing life’s challenges. We believe in the power of resilience and the human spirit. Learn more about us and join our mission to make a difference.
      </p>
      <button @click="navigateTo('about-us')">Learn More</button>
    </section>

    <!-- Featured Content Section -->
    <section class="featured-content">
      <h2 class="sub-heading">Featured Stories</h2>
      <div class="stories-carousel">
        <div v-for="story in featuredStories" :key="story.id" class="story">
          <h3 class="highlight">{{ story.title }}</h3>
          <p>{{ story.excerpt }}</p>
          <button @click="readStory(story.id)">Read More</button>
        </div>
      </div>
    </section>

    <!-- Community Highlights Section -->
    <section class="community-highlights">
      <h2 class="sub-heading">Join the Conversation</h2>
      <p>
        Be part of a supportive community where you can connect, share, and grow together. Check out our forums and upcoming events.
      </p>
      <button @click="navigateTo('community')">Explore Community</button>
      <button @click="navigateTo('events')">View Events</button>
    </section>

    <!-- Testimonials Section -->
    <section class="testimonials">
      <h2 class="sub-heading">What People Are Saying</h2>
      <div v-for="testimonial in testimonials" :key="testimonial.id" class="testimonial">
        <blockquote class="note">{{ testimonial.quote }}</blockquote>
        <p>- {{ testimonial.author }}</p>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "HomePage",
  data() {
    return {
      featuredStories: [
        { id: 1, title: "Overcoming Adversity", excerpt: "How I turned my struggles into success..." },
        { id: 2, title: "A Journey to Self-Love", excerpt: "Discovering the beauty of being me..." },
      ],
      testimonials: [
        { id: 1, quote: "Fallen Angels gave me hope when I felt lost.", author: "Alex T." },
        { id: 2, quote: "I found a community that truly understands.", author: "Jamie L." },
      ],
    };
  },
  methods: {
    navigateTo(route) {
      this.$router.push({ name: route });
    },
    readStory(id) {
      this.$router.push({ name: "story", params: { id } });
    },
  },
};
</script>

<style scoped>
  .Let-Them-Tasks {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    margin: 30px;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  }

  .Let-Them-Tasks h1, .Let-Them-Tasks h2 {
    color: #ffffff;
    font-weight: bold;
    margin-top: 30px;
    text-decoration: underline;
  }

  .Let-Them-Tasks h1 {
    font-size: 2rem;
    margin-bottom: 15px;
  }

  .Let-Them-Tasks h2 {
    font-size: 1.5rem;
    margin-bottom: 10px;
  }

  .Let-Them-Tasks p {
    font-size: 1rem;
    color: #ffffff;
    margin-bottom: 15px;
  }

  .Let-Them-Tasks ul {
    margin: 10px 0;
    padding-left: 20px;
  }

  .Let-Them-Tasks li {
    font-size: 1rem;
    color: #ffffff;
    margin-bottom: 10px;
  }

  .Let-Them-Tasks br {
    margin-bottom: 10px;
  }

  .Let-Them-Tasks .section-heading {
    font-size: 2rem;
    color: #ffffff;
    text-align: center;
    margin-bottom: 20px;
  }

  .Let-Them-Tasks .sub-heading {
    font-size: 1.2rem;
    color: #ffffff;
    margin-top: 20px;
    text-align: left;
  }

  .Let-Them-Tasks .highlight {
    color: #ffffff;
    font-weight: bold;
  }

  .Let-Them-Tasks .note {
    font-style: italic;
    color: #7f8c8d;
  }
</style>

