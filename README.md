<img src="https://raw.githubusercontent.com/rufusxxxx/rufusxxxx/main/.github/assets/gif2.gif" alt="CLOUDS GIF" width="1000">

<!DOCTYPE html>
<html lang="uk">
<head>
  <meta charset="UTF-8">
  <title>Про мене</title>
  <style>
    .menu-container {
      position: relative;
      display: inline-block;
      font-family: sans-serif;
    }

    .menu-button {
      cursor: pointer;
      padding: 8px 12px;
      background: #111;
      color: #fff;
      border-radius: 4px;
      user-select: none;
    }

    .dropdown {
      position: absolute;
      top: 110%;
      left: 0;
      background: #181818;
      padding: 8px;
      border-radius: 6px;
      display: none;
    }

    .dropdown img {
      width: 40px;
      height: 40px;
      cursor: pointer;
      display: block;
    }
  </style>
</head>
<body>

<div class="menu-container">
  <div class="menu-button" id="aboutBtn">Про мене</div>
  <div class="dropdown" id="dropdownMenu">
    <a href="https://open.spotify.com/user/31wh2mlekimceclhmxmlfcxnm3p4?si=14f003a4ef6544e6" target="_blank">
      <img src="https://wwwmarketing.scdn.co/img/structured-data/logo.png" alt="Spotify">
    </a>
  </div>
</div>

<script>
  const aboutBtn = document.getElementById('aboutBtn');
  const dropdownMenu = document.getElementById('dropdownMenu');

  aboutBtn.addEventListener('click', () => {
    dropdownMenu.style.display =
      dropdownMenu.style.display === 'block' ? 'none' : 'block';
  });

  // (необов’язково) закривати при кліку поза меню
  document.addEventListener('click', (e) => {
    if (!e.target.closest('.menu-container')) {
      dropdownMenu.style.display = 'none';
    }
  });
</script>

</body>
</html>

<!--
**rufusxxxx/rufusxxxx** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
