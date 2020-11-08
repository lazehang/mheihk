<template>
<section class="module">
  <div class="wrapper">
    <div class="pd row MHeiHK">
      <a id="section0" name="section0"></a>
      <div class="col-md-4 col-sm-12 col-xs-12 left_column">
        <p class="para_dash"></p>
        <br />
        <p class="color_txt about_topic text-red MHeiHK heavy">
          <font style="vertical-align: inherit"
            ><font style="vertical-align: inherit">網上商店新功能</font></font
          >
        </p>
      </div>
      <div class="col-md-8 col-sm-12 col-xs-12 description enquiry_content">
        <div class="pt-20">
          <div class="text-red">
            Headline
          </div>
          <p class="text-red">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam sit amet scelerisque ligula, quis consectetur libero. Cras pellentesque ac arcu et gravida. Vivamus a nibh sagittis nisi tempus accumsan non eu erat. In mollis non lectus id accumsan. Sed euismod, ante et sodales convallis, arcu neque ullamcorper nulla, et rhoncus mauris nisi fringilla lectus. Aliquam dictum convallis metus id pretium. Quisque consectetur lacus non lacus pellentesque ultricies. Nam lorem turpis, scelerisque sed orci ac, malesuada placerat arcu. In orci nunc, ullamcorper facilisis egestas vitae, molestie eu tortor. Vivamus rutrum sed neque non iaculis.
          </p>
          <button class="btn-red ml-auto">立即覲看</button>
        </div>
        <VideoList />
      </div>
    </div>
  </div>
</section>
</template>

<script>
import VideoList from './VideoList.vue'
export default {
  components: {
    VideoList
  }
}
</script>
