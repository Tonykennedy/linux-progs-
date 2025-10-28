<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>HTML Music Player</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <div class="player">
    <div class="cover">
      <img id="cover" src="" alt="cover" />
    </div>

    <div class="info">
      <div class="title" id="title">Title</div>
      <div class="artist" id="artist">Artist</div>

      <div class="controls">
        <button id="prev" title="Previous">⏮</button>
        <button id="play" title="Play/Pause">▶️</button>
        <button id="next" title="Next">⏭</button>

        <div class="spacer"></div>

        <button id="shuffle" title="Shuffle">🔀</button>
        <button id="repeat" title="Repeat">🔁</button>
      </div>

      <div class="progress-wrap">
        <span id="current-time">0:00</span>
        <input type="range" id="progress" min="0" max="100" value="0" />
        <span id="duration">0:00</span>
      </div>

      <div class="volume-wrap">
        <button id="mute" title="Mute">🔊</button>
        <input type="range" id="volume" min="0" max="1" step="0.01" value="1" />
      </div>
    </div>

    <div class="playlist" id="playlist"></div>
  </div>

  <audio id="audio" preload="metadata"></audio>

  <script src="script.js"></script>
</body>
</html>
