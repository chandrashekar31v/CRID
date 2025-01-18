<script lang="ts">
  import banner1 from "../resources/images/banner1.png";
  import banner2 from "../resources/images/banner2.png";
  import banner3 from "../resources/images/banner3.png";
  let imageList: any = {
    1: [
      banner1,
      "altImage1",
      "CRID is your partner in success.Strategic Partnerships for Agile IT & HR Excellence",
    ],
    2: [
      banner2,
      "altImage2",
      "Innovative IT & HR Solutions for Success.Empower Your Team with Proven IT & HR Strategies",
    ],
    3: [
      banner3,
      "altImage3",
      "Empowering Business Through IT & HR.Unlocking Your Business Potential Through Comprehensive IT & HR Services",
    ],
  };

  $: index = 1;
  $: image_url = imageList[index];

  setInterval(() => {
    if (index === 3) {
      index = 0;
    } else {
      index += 1;
    }
  }, 3000);
</script>

<div
  class="w-full h-[600px] bg-no-repeat bg-right-bottom bg-slate-200"
  style="background-image: url({image_url[0]})"
>
  <div class="flex justify-center items-center w-2/4 h-5/6">
    <div class="h-fit p-8">
      <h1 class="text-blue-600 font-extrabold text-6xl p-2">{image_url[2].split(".")[0]}</h1>
      <h3 class="text-3xl font-bold p-2">{image_url[2].split(".")[1]}</h3>
    </div>
  </div>
  <button
    class="border-2 bg-blue-600 px-4 py-2 rounded-lg text-white mt-10 ml-20 hover:bg-blue-800"
    >GET STARTED</button
  >
</div>
