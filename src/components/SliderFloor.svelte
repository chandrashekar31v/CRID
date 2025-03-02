<script lang="ts">
  import banner1 from "../resources/images/banner1.png";
  import banner2 from "../resources/images/banner2.png";
  import banner3 from "../resources/images/banner3.png";
  let imageList: any = {
    1: [
      banner1,
      "altImage1",
      "CIRD is your partner in success.Strategic Partnerships for Agile IT & HR Excellence",
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

<div class="w-screen md:h-[600px] h-[300px] bg-slate-200">
  <div
  class="bg-no-repeat px-4 md:bg-right-bottom"
  style="background-image: url({image_url[0]})"
>
  <div class="flex justify-center items-center md:w-2/4 w-3/4 h-[200px] md:h-5/6 ">
    <div class="h-fit md:p-8">
      <h1 class="text-blue-600 font-extrabold md:text-6xl text-2xl md:p-2">{image_url[2].split(".")[0]}</h1>
      <h3 class="md:text-3xl text-xl font-bold md:p-2">{image_url[2].split(".")[1]}</h3>
    </div>
  </div>
  <button
    class="border-2 bg-blue-600 md:px-4 px-3 py-2 rounded-lg text-white my-10 md:ml-20 hover:bg-blue-800 text-xs md:text-lg"
    >GET STARTED</button
  >
</div>
</div>

