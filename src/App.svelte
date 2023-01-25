<script>
  import Attribution from "./components/Attribution.svelte";
  import Info from "./components/Info.svelte";
  import Envelope from "./svg/Envelope.svelte";
  import LinkedIn from "./svg/LinkedIn.svelte";
</script>

<main class="card">
  <img
    src="/assets/laura-smith.jpg"
    alt="Laura Smith"
    class="card__profile"
    width="400"
    height="500"
  />
  <div class="card__container">
    <div class="text-align:center">
      <h1>Laura Smith</h1>
      <p class="card__job margin-top:0">Frontend Developer</p>
      <a href="/" class="card__website">laurasmith.website </a>
    </div>
    <div class="card__contact">
      <a href="/" class="card__button card__button--white">
        <Envelope className="card__icon" ariaHidden="true" />
        Email
      </a>
      <a href="/" class="card__button card__button--blue">
        <LinkedIn className="card__icon" ariaHidden="true" />
        LinkedIn
      </a>
    </div>
    <div class="card__text">
      <Info
        title="About"
        description="I am a frontend developer with a particular interest in making
        things simple and automating daily tasks. I try to keep up with
        security and best practices. I am always looking for new things to
        learn."
      />
      <Info
        title="Interests"
        description="Food expert. Music scholar. Reader. Internet fanatic. Bacon buff.
        Entrepreneur. Travel geek. Pop culture ninja. Coffee fanatic."
      />
    </div>
  </div>
  <div class="card__social-media">
    <a href="/" aria-label="Twitter">
      <!-- prettier-ignore -->
      <svg class="card__social-icon" width="24" height="28" viewBox="0 0 24 28" aria-hidden="true" focusable="false"><path d="M20 9.531a6.887 6.887 0 0 1-1.891.531 3.313 3.313 0 0 0 1.453-1.828 6.547 6.547 0 0 1-2.094.797A3.253 3.253 0 0 0 15.077 8a3.28 3.28 0 0 0-3.281 3.281c0 .25.016.516.078.75a9.324 9.324 0 0 1-6.781-3.437 3.33 3.33 0 0 0-.453 1.656c0 1.141.531 2.141 1.422 2.734-.547-.016-1.062-.172-1.563-.406v.031c0 1.594 1.203 2.922 2.703 3.219-.281.078-.5.125-.797.125-.203 0-.406-.031-.609-.063a3.3 3.3 0 0 0 3.063 2.281A6.607 6.607 0 0 1 4 19.53a9.351 9.351 0 0 0 5.031 1.469c6.031 0 9.344-5 9.344-9.344 0-.141 0-.281-.016-.422A6.31 6.31 0 0 0 20 9.53zM24 6.5v15c0 2.484-2.016 4.5-4.5 4.5h-15A4.502 4.502 0 0 1 0 21.5v-15C0 4.016 2.016 2 4.5 2h15C21.984 2 24 4.016 24 6.5z"/></svg>
    </a>
    <a href="/" aria-label="Facebook">
      <!-- prettier-ignore -->
      <svg class="card__social-icon" width="24" height="28" viewBox="0 0 24 28" aria-hidden="true" focusable="false"><path d="M19.5 2C21.984 2 24 4.016 24 6.5v15c0 2.484-2.016 4.5-4.5 4.5h-2.938v-9.297h3.109l.469-3.625h-3.578v-2.312c0-1.047.281-1.75 1.797-1.75L20.265 9V5.766c-.328-.047-1.469-.141-2.781-.141-2.766 0-4.672 1.687-4.672 4.781v2.672H9.687v3.625h3.125V26H4.499a4.502 4.502 0 0 1-4.5-4.5v-15c0-2.484 2.016-4.5 4.5-4.5h15z"/></svg>
    </a>
    <a href="/" aria-label="Instagram">
      <!-- prettier-ignore -->
      <svg class="card__social-icon" width="24" height="28" viewBox="0 0 24 28" aria-hidden="true" focusable="false"><path d="M16 14c0-2.203-1.797-4-4-4s-4 1.797-4 4 1.797 4 4 4 4-1.797 4-4zm2.156 0c0 3.406-2.75 6.156-6.156 6.156S5.844 17.406 5.844 14 8.594 7.844 12 7.844s6.156 2.75 6.156 6.156zm1.688-6.406c0 .797-.641 1.437-1.437 1.437S16.97 8.39 16.97 7.594s.641-1.437 1.437-1.437 1.437.641 1.437 1.437zM12 4.156c-1.75 0-5.5-.141-7.078.484-.547.219-.953.484-1.375.906s-.688.828-.906 1.375c-.625 1.578-.484 5.328-.484 7.078s-.141 5.5.484 7.078c.219.547.484.953.906 1.375s.828.688 1.375.906c1.578.625 5.328.484 7.078.484s5.5.141 7.078-.484c.547-.219.953-.484 1.375-.906s.688-.828.906-1.375c.625-1.578.484-5.328.484-7.078s.141-5.5-.484-7.078c-.219-.547-.484-.953-.906-1.375s-.828-.688-1.375-.906C17.5 4.015 13.75 4.156 12 4.156zM24 14c0 1.656.016 3.297-.078 4.953-.094 1.922-.531 3.625-1.937 5.031s-3.109 1.844-5.031 1.937c-1.656.094-3.297.078-4.953.078s-3.297.016-4.953-.078c-1.922-.094-3.625-.531-5.031-1.937S.173 20.875.08 18.953C-.014 17.297.002 15.656.002 14s-.016-3.297.078-4.953c.094-1.922.531-3.625 1.937-5.031s3.109-1.844 5.031-1.937c1.656-.094 3.297-.078 4.953-.078s3.297-.016 4.953.078c1.922.094 3.625.531 5.031 1.937s1.844 3.109 1.937 5.031C24.016 10.703 24 12.344 24 14z"/></svg>
    </a>
    <a href="/" aria-label="GitHub">
      <!-- prettier-ignore -->
      <svg class="card__social-icon" width="24" height="28" viewBox="0 0 24 28" aria-hidden="true" focusable="false"><path d="M8.109 18.75c.031-.047.016-.141-.047-.203-.078-.063-.172-.078-.219-.031-.031.047-.016.141.047.203.078.063.172.078.219.031zm-.437-.641c-.047-.063-.125-.094-.187-.063-.047.031-.047.125 0 .187.063.078.141.109.187.078.047-.031.047-.125 0-.203zm-.641-.625c.016-.031-.016-.094-.078-.125-.047-.016-.109-.016-.125.031-.031.047 0 .094.063.125.063.016.125.016.141-.031zm.328.36c.031-.031.031-.109-.031-.156-.047-.063-.125-.078-.156-.047-.047.047-.031.109.016.172.047.047.125.078.172.031zm1.344 1.172c.016-.063-.047-.141-.141-.172s-.172 0-.203.063c-.016.063.047.141.141.172s.172 0 .203-.063zm.656.047c0-.063-.078-.125-.187-.125-.094 0-.156.063-.156.125s.078.125.172.125.172-.063.172-.125zm.61-.11c-.016-.063-.109-.094-.203-.078s-.156.078-.141.141.094.109.187.094.156-.094.156-.156zM20 14c0-4.422-3.578-8-8-8s-8 3.578-8 8c0 3.531 2.297 6.531 5.469 7.594.406.078.547-.172.547-.391 0-.187 0-.812-.016-1.484 0 0-2.219.484-2.688-.953 0 0-.359-.922-.891-1.156 0 0-.719-.5.063-.5 0 0 .781.063 1.219.828.703 1.234 1.875.875 2.328.672.078-.516.281-.875.516-1.078-1.781-.203-3.656-.891-3.656-3.953 0-.875.313-1.578.828-2.141-.078-.203-.359-1.016.078-2.125.672-.203 2.203.828 2.203.828.641-.187 1.313-.266 2-.266s1.359.078 2 .266c0 0 1.531-1.031 2.203-.828.438 1.109.156 1.922.078 2.125.516.562.828 1.266.828 2.141 0 3.078-1.875 3.75-3.656 3.953.281.25.547.734.547 1.484 0 1.062-.016 1.922-.016 2.188 0 .219.141.469.547.391C17.703 20.533 20 17.533 20 14.001zm4-7.5v15c0 2.484-2.016 4.5-4.5 4.5h-15A4.502 4.502 0 0 1 0 21.5v-15C0 4.016 2.016 2 4.5 2h15C21.984 2 24 4.016 24 6.5z"/></svg>
    </a>
  </div>
</main>
<Attribution />

<style>
  .card {
    max-width: 30rem;
    background-color: var(--very-dark-blue-100);
    border-radius: 1rem;
    overflow: hidden;
  }

  .card__profile {
    width: 100%;
    max-height: 30rem;
    object-fit: cover;
  }

  .card__container {
    padding: 1.5rem;
  }

  .card__job {
    color: var(--dark-orange);
    margin-bottom: 1.5rem;
  }

  .card__contact {
    display: flex;
    justify-content: center;
    gap: 0.5rem;
    flex-wrap: wrap;
    margin-top: 1.5rem;
  }

  .card__button {
    flex-grow: 1;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 1rem 2rem;
    text-decoration-color: transparent;
    border-radius: 0.5rem;
  }

  :global(.card__icon) {
    margin-right: 0.6rem;
  }

  .card__button--white {
    background-color: var(--white);
    color: var(--very-dark-gray);
  }

  .card__button--blue {
    background-color: var(--blue);
    color: var(--white);
  }

  .card__text {
    margin-top: 3rem;
    margin-bottom: 3rem;
  }

  .card__social-media {
    display: flex;
    justify-content: center;
    gap: 1.5rem;
    padding: 2rem;
    background-color: var(--very-dark-blue-200);
  }

  .card__social-icon {
    display: inline-block;
    width: 2rem;
    height: auto;
  }
</style>
