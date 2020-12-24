<template>
    <div id="galleryImage">
        <div id=imgdiv :style="{ backgroundImage: 'url(' + fullpath + ')' }">

        </div>
    </div>
</template>

<script>
export default {
    name: "GalleryImage",
    props: {
        file: String,
        tags: Array,
    },
    computed: {
        fullpath () {
            return require('@/assets/gallery/' + this.file);
        //},
        //urlpath () {
            //return url('~@/assets/gallery/' + this.file);
        }
    }
}
</script>

<style scoped>
#galleryImage {
    width: 300px;
    height: 300px;
}

#imgdiv {
    width: 100%;
    height: 100%;
    background-size: contain;
    background-repeat: no-repeat;
    background-position: center;
}

</style>
