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
        <p>Every Thursday we come together as a large group to spend time in fellowship with each other, as we enjoy Jesus together. This year we're moving towards a em group format, where we can encourage each other and explore truth together. Everyone is welcome, regardless of your spiritual background or lack thereof. If you are only able to attend a meeting once a week we usually encourage people to come to the Thursday meetings because it is a really good way to experience the Church, the body of Christ, as we come together with complimentary gifts that all point to God.</p>
      </div>
      <div class="content-group">
        <h3>Bridging the Divide</h3>
        <em class="meeting-info-text">
          Meeting Info
          <br />Thursdays 6-7:30PM, Location TBD
        </em>
        <p>Briding the Divide is a weekly partnership event with the Islamic Society of Northeastern, where students from both religions can come togehter in the pursuit of truth.</p>
      </div>
      <div class="content-group">
        <h3>Study Squared</h3>
        <em class="meeting-info-text">
          Meeting Info
          <br />Saturdays at 10:30AM at Kim's Apartment. Send Kim an email for the address! (minch.k@husky.neu.edu)
        </em>
        <p>Study Squared is a great way to start off your weekend. We start with a bible study in the book of Daniel, and then around 11:30AM switch over to hanging out and doing homework together. No homework is necessary to attend!</p>
      </div>
      <div class="content-group">
        <h3>Mens Fellowship</h3>
        <em class="meeting-info-text">
          Meeting Info
          <br />Time and Date being determined, but email Patrick for more info (mcgrath.p@husky.neu.edu), and fill out this
          <a
            href="https://forms.gle/4M1Hwu5dGNsAdKBC8"
          >availability form</a>!
        </em>
        <p>
          Jesus tells us that where two or three are gathered in His name, He is there with us. We believe that this is truth, and think that it is important for us to gather to seek the Lord together. We will be meeting weekly to encourage each other, spend time in the Word, and grow closer to the Lord together and turn our eyes away from the temporary things of this world, and focus on something much greater than ourselves.
          If you're interested in coming please fill out this
          <a
            href="https://forms.gle/4M1Hwu5dGNsAdKBC8"
          >availability form.</a>
          <br />
          <br />We'll also be having other gatherings throughout the semester, with more information about them at our weekly large group meetings on Thursdays.
        </p>
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
        'Thursday Janaury 23, 2020: Social Justice Resource Center @ 106 St. Stephen Street',
      alert: true
    }
  }
}
</script>
