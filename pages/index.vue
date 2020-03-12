<template>
  <div class="main">
    <div class="homepage__introduction">
      <div class="container">
        <div class="homepage__introduction-wrapper">
          <h1>
            Agape Christian Fellowship
            <br />
            <em class="heading-subtitle">Cru Boston</em>
          </h1>
          <blockquote>at Northeastern University</blockquote>
        </div>
      </div>
      <div class="homepage__introduction-verse">
        <div class="container">
          <em>
            This is real love - not that we loved God, but that he loved us and sent his Son as a sacrifice to take away our sins.
            <br />
            <small>1 John 4:10</small>
          </em>
        </div>
      </div>
      <div v-if="alert" class="homepage__alert">
        <div class="container">
          Updated Thursday Meeting Information
          <br />
          <br />
          {{ meeting_info }}
        </div>
      </div>
    </div>
    <section class="container">
      <div class="content-group">
        <h3>About</h3>
        <p>Agape Christian Fellowship is a group of students at and nearby Northeastern University that are pursuing a relationship with Jesus together. We believe that God made and loves us, and wants to have a relationship with us, and because of Jesus Christ, we can enter into that relationship.</p>
      </div>
      <hr />
      <div class="content-group">
        <h3>Online Fellowship</h3>
        <em class="meeting-info-text">
          Meeting Info
          <br />
          {{ meeting_info }}
        </em>
        <p>
          Northeastern University has advised that student organizations no longer meet in person to reduce the chances of the Coronavirus (COVID-19) spreading between people. In response to that we will be having fellowship online (audio or video conference) this week. We're going to be taking things week by week, so check back each week for more information, and to confirm that we are still meeting.
          <br />
          <br />
          Do not feel obliged to join, but it will be a time for those who are interested to gather together online and have fellowship with each other.
        </p>
      </div>
      <div class="content-group">
        <h3>Abide in Christ - A Month Long Focus</h3>
        <em class="meeting-info-text">
          Content
          <br />
          <a href="/introduction.pdf"> PDF With Introduction and Schedule </a>
        </em>
        <p>
          For the four weeks leading up to Good Friday we will be taking a special look at what it means to Abide in Christ. Each week there will be a special focus with specific passages in the Bible that you can read throughout the week. Each day of the week there will be something for you to engage with, whether its a devotional posted on our social media
        </p>
        <div class="abide-introduction-wrapper">
          <img class="abide-introduction-image" src="/introduction.png">
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  data: function() {
    return {
      upcomingEvents: [],
      meeting_info:
        'Thursdays at 7:30PM, Online Audio or Video Conference. Link posted here and on social media at 7:15pm on Thursday.',
      alert: true
    }
  }
}
</script>
