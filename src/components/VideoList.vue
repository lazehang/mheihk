<template>
    <div class="row">
        <Video
            v-for="(video, i) in list"
            :key="i"
            :title="video.title"
            :thumbnail="video.thumbnail"
        />
    </div>
</template>

<script>
import Video from './Video.vue'
export default {
    components: {
        Video
    },
    data() {
        return {
            list: [
                {
                    title: '無紙二維碼換領產品',
                    url: 'https://www.youtube.com/embed/Qsquj7Ulrsw',
                    thumbnail: 'https://img.youtube.com/vi/Qsquj7Ulrsw/maxresdefault.jpg',
                },
                {
                    title: '無紙二維碼換領產品',
                    url: 'https://www.youtube.com/embed/Qsquj7Ulrsw',
                    thumbnail: 'https://img.youtube.com/vi/Qsquj7Ulrsw/maxresdefault.jpg',
                },
                {
                    title: '無紙二維碼換領產品',
                    url: 'https://www.youtube.com/embed/Qsquj7Ulrsw',
                    thumbnail: 'https://img.youtube.com/vi/Qsquj7Ulrsw/maxresdefault.jpg',
                }
            ]
        }
    }
}
</script>
