<template>
    <div class="col-12 col-md-4 yt-video-item">
        <div class="text-red title">{{ title }}</div>
        <div class="yt-thumbnail">
            <img :src="thumbnail" />
        </div>
        <div>
            <button class="btn-red m-auto" @click="toggle">立即覲看</button>
        </div>
        <div v-if="showModal" class="yt-modal">
            <div class="yt-inner">
                <div class="yt-close" @click="toggle"><i class="glyphicon glyphicon-remove text-white" /></div>
                <div class="embed-container">
                    <iframe src="https://www.youtube.com/embed/Qsquj7Ulrsw" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        title: {
            type: String,
            default: ''
        },
        thumbnail: {
            type: String,
            default: ''
        }
    },
    data() {
        return {
            showModal: false
        }
    },
    methods: {
        toggle() {
            this.showModal = !this.showModal
        }
    }
}
</script>
<style lang="scss" scoped>
.yt-video-item {
    padding: 0 15px;
    margin-bottom: 15px;
    .title {
        padding-top: 50px;
        padding-bottom: 20px;
    }
}
.yt-thumbnail {
    padding-bottom: 20px;
    img {
        max-width: 100%;
        border: 1px solid black;
    }
}
.yt-modal {
    position: fixed;
    z-index: 1000;
    top: 0;
    left: 0;
    height: 100vh;
    width: 100vw;
    background-color: rgba(0, 0, 0, 0.7);
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    .yt-inner {
        background-color: #fff;
        padding: 40px;
        max-width: 1000px;
        width: 100%;
        margin: 50px;
        position: relative;
        @media (max-width: 767px) {
            margin: 0px;
            padding: 20px;
        }
        .embed-container {
            position: relative;
            padding-bottom: 56.25%;
            height: 0;
            overflow: hidden;
            max-width: 100%;
        }
        .embed-container iframe,
        .embed-container object,
        .embed-container embed {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
        }
        .yt-close {
            position: absolute;
            bottom: 100%;
            left: 100%;
            margin: 10px;
            font-size: 35px;
            cursor: pointer;
            @media (max-width: 767px) {
                margin: 0px;
                left: auto;
                right: 0;
            }
        }
    }
}
</style>