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
          Updated Thursday Meeting Location
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
        <h3>Weekly Large Group Meetings</h3>
        <em class="meeting-info-text">
          Meeting Info
          <br />
          {{ meeting_info }}
        </em>
        <p>Every Thursday we come together as a large group to spend time in fellowship with each other, as we enjoy Jesus together. Everyone is welcome regardless of your spiritual background or lack thereof. If you are only able to attend a meeting once a week we usually encourage people to come to the Thursday meetings because it is a really good way to experience the Church, the body of Christ, as we come together with complimentary gifts that all point to God.</p>
      </div>
      <div class="content-group">
        <h3>Bridging the Divide</h3>
        <em class="meeting-info-text">
          Meeting Info
          <br />Thursdays 6-7:30PM, Location TBD. Contact Heather at novak.h@husky.neu.edu for more information!
        </em>
        <p>Briding the Divide is a partnership event with the Islamic Society of Northeastern, where students from both religions can come together in the pursuit of truth.</p>
      </div>
      <div class="content-group">
        <h3>Study Squared</h3>
        <em class="meeting-info-text">
          Meeting Info
          <br />Saturdays at 10:30AM at Kim's Apartment. Send Kim an email for the address! (minch.k@husky.neu.edu)
        </em>
        <p>Study Squared is a great way to start off your weekend. We start with a bible study in the book of Daniel, and then around 11:30AM switch over to hanging out and doing homework together. No homework is necessary to attend!</p>
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
        'Thursday February 6 at 7:30PM: Social Justice Resource Center @ 106 St. Stephen Street',
      alert: true
    }
  }
}
</script>
