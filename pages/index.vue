<template>
  <div class="main">
    <div class="homepage__introduction">
      <div class="container">
        <h1>Agape Christian Fellowship
          <br>
          <em class="heading-subtitle">Part of Cru Boston</em>
        </h1>
        <blockquote>at Northeastern University</blockquote>
      </div>
    </div>
    <section class="container">
      <div class="content-group">
        <h3>What we're about</h3>
        <p>Agape Christian Fellowship is a group of students at and nearby Northeastern University that are pursuing a relationship with Jesus together. We believe that God made and loves us, and wants to have a relationship with us, and because of Jesus Christ, we can enter into that relationship.</p>
      </div>
      <div class="content-group">
        <h3>In the works</h3>
        <div class="card-row">
          <image-card
            v-for="initiative in initiatives"
            :key="initiative.id"
            :description="initiative.description"
            :image-url="initiative.imageUrl"
            :link-path="initiative.linkPath"
          />
        </div>
      </div>
      <div class="content-group">
        <h3>Upcoming initiatives</h3>
        <p
          v-for="event in upcomingEvents"
          :key="event.id"
        ></p>
      </div>
    </section>
  </div>
</template>

<script>
import ImageCard from '@/components/ImageCard.vue'

export default {
  components: {
    ImageCard
  },
  data: function() {
    return {
      upcomingEvents: [],
      initiatives: [
        {
          id: 1,
          description: 'Bible Study',
          linkPath: '#',
          imageUrl:
            'https://images.unsplash.com/photo-1509559449230-59c948a61f51?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=3900&q=80'
        },
        {
          id: 2,
          description: 'Thursday Meetings',
          linkPath: '#',
          imageUrl:
            'https://images.unsplash.com/photo-1509559449230-59c948a61f51?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=3900&q=80'
        },
        {
          id: 3,
          description: 'Prayer Meetings',
          linkPath: '#',
          imageUrl:
            'https://images.unsplash.com/photo-1509559449230-59c948a61f51?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=3900&q=80'
        }
      ]
    }
  }
}
</script>
