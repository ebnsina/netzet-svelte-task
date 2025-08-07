<script lang="ts">
  import Banner from "$lib/assets/hero@2x.png";
  import BannerDesktop from "$lib/assets/hero-desk@2x.png";
  import Logo from "$lib/assets/logo.svg";
  import LogoDesktop from "$lib/assets/logo-desktop.svg";
  import { features } from "$lib/data/features";
  import { Menu } from "lucide-svelte";
</script>

<main class="relative w-full min-h-screen pb-10">
  <div
    class="bg-[linear-gradient(90deg,rgba(252,0,78,1)_0%,rgba(16,203,224,1)_100%)] p-5 md:p-2.5 w-full"
  >
    <div class="text-center leading-none">
      <span
        class="font-extrabold text-brand-cyan text-base md:text-[22px] leading-none"
        >🚀 FRESH BEGINNINGS SALE:</span
      >
      <span class="font-semibold text-white text-sm md:text-[22px] leading-none"
        >Extra 25% OFF, Limited Spots - start your journey today!
      </span>
    </div>
  </div>

  <div class="w-full relative">
    <header
      class="max-w-5xl mx-auto sm:px-6 xl:px-0 flex w-full md:pt-[35px] relative"
    >
      <div class="flex-1 flex md:justify-start items-center">
        <div class="hidden md:block">
          <img class="" src={LogoDesktop} alt="Logo" />
        </div>
      </div>
      <nav class="hidden md:flex text-white text-lg font-medium mr-[17px] -mt-1">
        <ul class="flex space-x-10">
          <li>
            <a class="text-lg font-semibold text-brand-gray leading-none" href="/about">About us</a>
          </li>
          <li>
            <a class="text-lg font-semibold text-brand-gray leading-none" href="/contact">Contact</a>
          </li>
        </ul>
      </nav>
      <Menu
        class="absolute right-[24px] top-[26px] md:hidden cursor-pointer z-20"
        aria-label="Menu"
      />
    </header>

    <div
      class="max-w-5xl mx-auto overflow-y-hiddens sm:px-6 xl:px-0 relative flex flex-col md:flex-row md:items-center md:justify-between gap-6 md:gap-0"
    >
      <div class="md:hidden w-full relative">
        <div class="absolute left-1/2 -translate-x-1/2 z-20 mt-4 md:mt-0">
          <img src={Logo} alt="Logo" class="md:hidden w-[105px] h-[45px]" />
        </div>
        <div class="flex justify-center w-full relative z-0">
          <img class="md:hidden w-full" alt="Hero mockup" src={Banner} />
        </div>
      </div>

      <div
        class="md:w-2/3 w-full flex flex-col items-center md:items-start z-10 relative"
      >
        <div
          class="flex flex-col items-center md:items-start pb-0 px-4 md:px-0"
        >
          <div class="max-w-[350px] md:max-w-[516px] md:mt-[57px]">
            <h1
              class="z-10 w-full font-urbanist-sans font-extrabold md:font-bold text-white text-[25px] md:text-[35px] text-center md:text-left -mt-[86px] md:-mt-0 leading-[1.15]"
            >
              Want to Turn Social Media Into a Profitable Career?
            </h1>
            <h2
              class="mt-1 [text-shadow:0px_4px_4px_#fc004e] font-urbanist-sans font-extrabold md:font-bold text-brand-cyan text-[25px] md:text-[35px] text-center md:text-left leading-[1.1]"
            >
              Discover your way to success with Fametonic:
            </h2>
          </div>

          <ul
            class="flex flex-col items-start space-y-2.5 md:space-y-[13px] max-w-[350px] md:max-w-[516px] mt-[25px] md:mt-4"
          >
            {#each features as { icon, text }}
              <li
                class="flex items-center gap-2.5 w-full"
              >
                <span class="font-medium text-[22px] leading-none">{icon}</span>
                <span class="font-normal md:font-semibold text-base leading-[22px]">{text}</span>
              </li>
            {/each}
          </ul>

          <!-- Footer mobile -->
          <footer
            class="flex flex-col w-full max-w-xs items-center mt-[22px] md:hidden"
          >
            <p
              class="w-full font-medium text-[#aaaaaa] text-xs text-center leading-[1.15]"
            >
              By clicking &quot;Get Started&quot;, you agree with Terms and
              Conditions, Privacy Policy, Subscription Terms
            </p>
            <p
              class="w-full font-medium text-[#aaaaaa] text-[10px] text-center mt-[20px] leading-[1.15]"
            >
              Fametonic 2025 ©All Rights Reserved.
            </p>
          </footer>
        </div>

        <div
          class="flex flex-col w-full items-center md:items-start justify-end px-4 md:px-0 mt-10 md:mt-[30px]"
        >
          <div
            class="flex flex-col items-center md:items-start md:max-w-[313px] w-full"
          >
            <button
              class="flex items-center justify-center px-10 py-2 w-full bg-brand-red rounded-[10px] shadow-[2px_2px_10px_#00e7f9]"
            >
              <span
                class="font-urbanist-sans font-bold text-white text-lg md:text-xl leading-none whitespace-nowrap"
              >
                GET STARTED
              </span>
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="24"
                height="24"
                viewBox="0 0 24 24"
                fill="none"
                stroke="currentColor"
                stroke-width="3"
                stroke-linecap="round"
                stroke-linejoin="round"
                class="lucide lucide-chevron-right-icon lucide-chevron-right"
                ><path d="m9 18 6-6-6-6" /></svg
              >
            </button>
            <p
              class="w-full font-normal text-white text-xs text-center leading-4 mt-2.5"
            >
              1-minute quiz for personalized Insights
            </p>
          </div>

          <!-- Footer Desktop -->
          <footer class="hidden md:flex flex-col max-w-[516px] items-start mt-[30px]">
            <p
              class="w-full font-medium text-[#ABABAB] text-xs text-left leading-none"
            >
              By clicking &quot;Get Started&quot;, you agree with Terms and
              Conditions, Privacy Policy, Subscription Terms
            </p>
            <p
              class="mt-3 w-full font-medium text-[#ABABAB] text-[10px] text-left leading-none"
            >
              Fametonic 2025 ©All Rights Reserved.
            </p>
          </footer>
        </div>
      </div>
    </div>

    <div
      class="absolute right-[144px] top-[80px] w-auto md:flex justify-end lg:z-0 hidden"
    >
      <img
        class="w-[666px] h-auto max-h-[800px] object-contain"
        alt="Hero mockup"
        src={BannerDesktop}
      />
    </div>
  </div>
</main>
