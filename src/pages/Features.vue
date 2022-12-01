<script>
import FeatureVue from "../components/Feature.vue";
import ButtonVue from "../components/Button.vue";
export default {
  components: { FeatureVue, ButtonVue },
};
</script>

<template>
  <div id="features" class="bg-[#5267DF] text-white pt-20">
    <!-- ? Heading section -->
    <section class="pt-32 flex flex-col items-center text-center mx-10">
      <h1 class="text-4xl font-normal">Features</h1>
      <p class="text-lg text-gray-400 pt-4">
        From professional podcasting to music recording, gaming and even sound
        for video, Yeti takes your <br />
        projects to the heights of studio quality.
      </p>
    </section>
    <!-- todo Items Section -->
    <!-- * Feature # 1 -->
    <div>
      <feature-vue heading="Full control of the recording">
        <template v-slot:image>
          <img
            src="../assets/images/feature1.png"
            width="500"
            height="500"
            class="z-10"
            alt="Mic"
          />
        </template>
        <template #content>
          <p class="pb-4 text-gray-400">
            Yeti features studio controls for headphone volume, directionality
            selection, instant mute and microphone gain - giving you control
            over all aspects of the recording process. <br /><br />
            The microphone is equipped with a 3.5-millimeter mini-jack for
            headphones that allows you to listen to what you are recording in
            real time, without latency.
          </p>
          <ButtonVue name="More Info" />
        </template>
      </feature-vue>
    </div>

    <!-- * Feature #2 -->

    <div>
      <div class="text-white flex justify-center items-center mt-16">
        <div class="flex flex-col items-center lg:flex-row md:py-20 lg:px-20">
          <div
            class="
              text-center
              lg:text-left
              py-10
              order-2
              lg:order-1
              w-9/12
              md:w-2/5
              lg:ml-36
              xl:ml-60
            "
          >
            <h1 class="text-3xl font-bold text-gray-200 pb-4">
              Innovation design facilitate registration
            </h1>
            <p class="pb-4 text-gray-400">
              The Yeti can be adjusted and rotated to suit the sound source,
              optimizing your sound quality. Once you've reached your desired
              angle, simply hand-tighten its adjustment knobs to keep it in
              place.
              <br /><br />
              The Yeti is a side-capture microphone, so you will get the best
              sound quality by facing it. The microphone can also be folded down
              for easy transport, or completely removed from its base for direct
              mounting on a microphone stand or the Radius II shock mount.
            </p>
            <ButtonVue name="More Info" />
          </div>
          <div class="w-[30%] flex justify-center lg:order-2">
            <img
              src="../assets/images/feature2.png"
              width="400"
              height="400"
              class="z-10"
              alt="Mic"
            />
          </div>
          <!-- todo Bg black Color Mic -->
          <div
            class="
              absolute
              lg:w-[40%]
              h-80
              bg-black
              right-0
              translate-y-40
              rounded-tl-full rounded-bl-full
            "
          ></div>
        </div>
      </div>
    </div>

    <!-- * Feature #3 -->
    <div>
      <feature-vue heading="Directional modes">
        <template #image>
          <img
            src="../assets/images/feature3.png"
            width="450"
            height="450"
            class="z-10 lg:relative lg:-top-20"
            alt="Mic"
          />
        </template>
        <template #content>
          <p class="pb-4 text-gray-400">
            Cardioïde Mode : Ideal for podcasts, game streaming, vocal
            performances, voice-overs and instruments. It records sound sources
            directly in front of it, giving a rich, full sound.
            <br />
            <br />
            Stereo Mode : Uses both left and right channels to capture a wide,
            realistic soundstage - ideal for recording acoustic guitar or choir.
          </p>
          <ButtonVue name="More Info" />
        </template>
      </feature-vue>
    </div>
    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
      <path
        fill="#"
        fill-opacity="1"
        d="M0,128L80,160C160,192,320,256,480,261.3C640,267,800,213,960,213.3C1120,213,1280,267,1360,293.3L1440,320L1440,320L1360,320C1280,320,1120,320,960,320C800,320,640,320,480,320C320,320,160,320,80,320L0,320Z"
      ></path>
    </svg>
  </div>
</template>
     

