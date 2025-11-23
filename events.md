---
layout: page
title: Events
permalink: /events
---

<div class="events-intro">
  <p>Check out our upcoming events and activities. You can also <a href="https://calendar.google.com/calendar/u/0?cid=ZjJvanMxczRhY3RycmJ2dGNlcWM1OWJsMXNAZ3JvdXAuY2FsZW5kYXIuZ29vZ2xlLmNvbQ" target="_blank">add this calendar to your Google Calendar</a>.</p>
</div>

<div class="calendar-wrapper">
  <div class="calendar-container">
    <iframe src="https://calendar.google.com/calendar/embed?src=f2ojs1s4actrrbvtceqc59bl1s%40group.calendar.google.com&ctz=Europe%2FBerlin&mode=AGENDA&showTitle=0&showNav=1&showDate=1&showPrint=0&showTabs=0&showCalendars=0&showTz=0&color=%230085A1&bgcolor=%23ffffff" style="border: 0" width="100%" height="700" frameborder="0" scrolling="yes"></iframe>
  </div>
</div>

<style>
.events-intro {
  margin: 0 0 40px 0;
}

.events-intro p {
  margin: 0 0 20px 0;
  font-size: 18px;
  color: #212529;
  line-height: 1.6;
}

.events-intro a {
  color: #0085A1;
  text-decoration: underline;
  font-weight: 600;
  transition: all 0.2s;
}

.events-intro a:hover {
  color: #006b84;
  text-decoration: none;
}

/* Calendar Wrapper */
.calendar-wrapper {
  margin: 0 0 40px 0;
}

.calendar-container {
  border: 3px solid #0085A1;
  border-radius: 8px;
  overflow: hidden;
  box-shadow: 0 0.5rem 1rem rgba(0, 133, 161, 0.15);
  background: white;
  transition: all 0.3s ease;
}

.calendar-container:hover {
  box-shadow: 0 0.75rem 1.5rem rgba(0, 133, 161, 0.25);
  transform: translateY(-2px);
}

.calendar-container iframe {
  display: block;
  background: white;
  min-height: 700px;
}

/* Responsive Design */
@media (max-width: 768px) {
  .events-intro p {
    font-size: 16px;
  }

  .calendar-container {
    border-radius: 0;
    border-left: 0;
    border-right: 0;
    border-width: 2px;
  }

  .calendar-container:hover {
    transform: none;
  }

  .calendar-container iframe {
    min-height: 600px;
    height: 600px;
  }
}

@media (min-width: 768px) {
  .events-intro p {
    font-size: 20px;
  }
}

/* Additional professional styling */
@media (min-width: 992px) {
  .calendar-container {
    border-radius: 12px;
  }

  .calendar-container iframe {
    min-height: 800px;
  }
}
</style>
