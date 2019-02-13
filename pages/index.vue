<template>
  <div class="main">
    <div
      class="homepage__introduction"
      :style="{'background-image': 'url(' + require('@/static/crossword.png') + ')'}"
    >
      <div class="container">
        <h1>
          Agape
          <br>Christian
          <br>Fellowship
        </h1>
        <h2>
          Loving God.
          <br>Loving Each Other.
          <br>Loving Our Campus.
        </h2>
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
            v-for="event in events"
            :key="event.id"
            :description="event.description"
            :image-url="event.imageUrl"
            :link-path="event.linkPath"
          />
        </div>
      </div>
      <div class="content-group">
        <h3>Upcoming events</h3>
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
