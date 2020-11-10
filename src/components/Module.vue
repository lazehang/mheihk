<template>
<section class="module">
  <div class="wrapper">
    <div class="pd row MHeiHK">
      <a id="section0" name="section0"></a>
      <div class="col-md-4 col-sm-12 col-xs-12 left_column">
      </div>
      <div class="col-md-8 col-sm-12 col-xs-12 description enquiry_content">
        <div>
          <div class="text-red pb-20">
            <span class="text-19 MHeiHK heavy">建立帳戶，立即享用全新功能！</span>
            <button class="btn-red ml-auto">立即覲看</button>
          </div>
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
