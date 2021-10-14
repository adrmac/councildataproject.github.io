<ul class="steps">
  <li>
    <span class="step-index">1</span>
    <span class="step-description">
      <strong>Gather Events</strong>
      Providing new event information to CDP processing pipelines can be
      as simple as providing <a class="cdp-link" href="https://councildataproject.github.io/cdp-backend/ingestion_models.html#minimal-event-data">a URL to a meeting recording</a>
      or as expansive as <a class="cdp-link" href="https://councildataproject.github.io/cdp-backend/ingestion_models.html#expanded-event-data-with-event-minutes-items">attaching all minutes items and vote information</a>.
      <br />
      <br />
      In many cases, gathering event information can be quite simple as hundreds of cities and 
      counties across the US <a class="cdp-link" href="https://granicus.com/solution/govmeetings/">all use the same system</a>
      for tracking municipal council meeting and legislation information.
      <br />
      <br />
      But even if your council doesn't use one of the commonly used tracking systems, as long as 
      some basic event information is provided to our tools, CDP will still work for you.
    </span>
  </li>

  <li>
    <span class="step-index">2</span>
    <span class="step-description">
      <strong>Transcribe and Process</strong>
      For each event our tools receive, our pipeline will either clean up and use the provided 
      closed caption files, or create transcripts using the event recording.
      <br />
      <br />
      We then process and store all provided minutes and legislative items, voting records, and 
      any attached documents, and update any council member and legislation status information.
    </span>
  </li>
  <li>
    <span class="step-index">3</span>
    <span class="step-description">
      <strong>Natural Language Search</strong>
      We understand that legal jargon can make following council action incredibly difficult.
      <br />
      <br />
      To solve this, every two days our tools will index all documents, legislation, and meeting 
      transcripts to enable plain text search throughout CDP systems.
    </span>
  </li>
</ul>

<style>
  .steps li {
    display: flex;
  }

  .steps .step-index { 
    position: relative;
    color: #2e2e2e;
    padding: 0 1.5em;
    font-family: 'Courier New', Courier, monospace;
  }

  .steps .step-description {
    padding: 0 1.5em 1.5em 1.5em;
    position: relative;
  }

  .steps .step-description::before {
    content: "";
    position: absolute;
    z-index: 1;
    left: 0;
    height: 100%;
    border-left: 1px #2e2e2e solid;
  }

  .steps li:last-child .step-description {
    padding: 0 1.5em 0 1.5em;
  }

  .steps strong {
    display: block;
    font-weight: bolder;
  }

  .steps { margin: 40px auto 40px auto; }
  .steps,
  .steps *::before,
  .steps *::after { box-sizing: border-box; }
</style>