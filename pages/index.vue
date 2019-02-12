<template>
  <section class="container">
    <div class="homepage__intro">
      <h1>Agape Christian Fellowship</h1>
      <p>Agape Christian Fellowship is a group of students at and nearby Northeastern University that are pursuing a relationship with Jesus together. We believe that God made and loves us, and wants to have a relationship with us, and because of Jesus Christ, we can enter into that relationship.</p>
      <h3>In the Works</h3>
      <div class="card-row">
        <image-card
          v-for="event in events"
          v-bind:key="event.id"
          v-bind:description="event.description"
          v-bind:imageUrl="event.imageUrl"
          v-bind:linkPath="event.linkPath"
        ></image-card>
      </div>
    </div>
    <div class="homepage__events">
      <h3>Upcoming Events</h3>
    </div>
  </section>
</template>

<script>
import ImageCard from '@/components/ImageCard.vue'

export default {
  components: {
    ImageCard
  },
  data: function() {
    return {
      events: [
        {
          id: 1,
          description: 'Bible Study',
          linkPath: '#',
          imageUrl:
            'https://images.unsplash.com/photo-1509559449230-59c948a61f51?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=3900&q=80'
        },
        {
          id: 2,
          description: 'Bible Study',
          linkPath: '#',
          imageUrl:
            'https://images.unsplash.com/photo-1509559449230-59c948a61f51?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=3900&q=80'
        },
        {
          id: 3,
          description: 'Bible Study',
          linkPath: '#',
          imageUrl:
            'https://images.unsplash.com/photo-1509559449230-59c948a61f51?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=3900&q=80'
        },
        {
          id: 4,
          description: 'Bible Study',
          linkPath: '#',
          imageUrl:
            'https://images.unsplash.com/photo-1509559449230-59c948a61f51?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=3900&q=80'
        }
      ]
    }
  }
}
</script>
