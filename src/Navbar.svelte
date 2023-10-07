<script>
  document.addEventListener('DOMContentLoaded', () => {
    const heading = document.querySelector('.sparkle-heading');
    const numSparkles = 20;

    function randomValue(min, max) {
      return Math.random() * (max - min) + min;
    }

    for (let i = 0; i < numSparkles; i++) {
      const sparkle = document.createElement('span');
      sparkle.classList.add('sparkle');
      sparkle.style.setProperty('--sparkle-translate-x', `${randomValue(-10, 105)}%`);
      sparkle.style.setProperty('--sparkle-translate-y', `${randomValue(-30, 100)}%`);
      sparkle.style.setProperty('--sparkle-size', `${randomValue(1, 5)}px`);
      sparkle.style.setProperty('--sparkle-opacity', `${randomValue(0.2, 1)}`);
      sparkle.style.setProperty('--sparkle-animation-delay', `${randomValue(0, 2)}s`);
      heading.appendChild(sparkle);
    }
  });



</script>

<main>
  <nav>
    <a href="#home" aria-label="logo" class="flex space-x-2 items-center">

      <h1>OpenVerse</h1>
  </a>
      

      
        
      <div class="menu-right">
        <a href="#" class="note">Want to contribute ? ... Join in!</a>
        <a href="https://forms.gle/9ruKMLksn98LVd4K9" target="_blank" class="btn">Add a Site</a>
      </div>
  </nav>
  <h1 class="sparkle-heading">Find Cool Open Source Projects!</h1>
  <p>Only the Best Projects gets Featured</p>

</main>

<style>
    main {
        display: flex;
        flex-direction: column;
        justify-content: flex-start;
        align-items: center;
    }
</style>