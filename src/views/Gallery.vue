<template>
    <div id="gallery">
        <h1>Gallery</h1>
        <div id="galleryLoop">
            <gallery-image v-for="image in images" :file=image.file />
        </div>
    </div>
</template>

<script>
import GalleryImage from "@/components/GalleryImage.vue";

export default {
    name: "Gallery",
    components: {
        GalleryImage,
    },
    data () {
        return {
            "images": [
                {
                    "file": "Picture1.jpg",
                    "tags": ["bird","robin","snow","christmas","red","brown","festive","winter","animal"]
                },
                {
                    "file": "Picture2.jpg",
                    "tags": ["tree","christmas","snow","green","fern","festive","winter","plant"]
                },
                {
                    "file": "Picture3.jpg",
                    "tags": ["reindeer","red","animal","christmas","candle","candle holder","tealight"]
                },
                {
                    "file": "Picture4.jpg",
                    "tags": ["christmas","candle","candle holder","tealight"]
                },
                {
                    "file": "Picture5.jpg",
                    "tags": ["candle","candle holder","tealight","tree","green","christmas","fern"]
                },
                {
                    "file": "Picture6.jpg",
                    "tags": ["candle holder","candle","plate","christmas","holly","green","red"]
                },
                {
                    "file": "Picture7.jpg",
                    "tags": ["candle","plate","candle holder","christmas","holly","green","red"]
                },
                {
                    "file": "Picture8.jpg",
                    "tags": ["wreath","holly","christmas","green","red","festive"]
                },
                {
                    "file": "Picture9.jpg",
                    "tags": ["tree","blue","fern","christmas","candle","holder"]
                },
                {
                    "file": "Picture10.jpg",
                    "tags": ["abstract","tree","black","blue","teal","leaf","marble","swirl"]
                },
                {
                    "file": "Picture11.jpg",
                    "tags": ["flower","daisy","plant","candle","holder","tealight","yellow","green","white"]
                }
            ]
        }
    }
}
</script>

<style scoped>
#galleryLoop {
    display: grid;
    margin: 0 auto;
    grid-gap: 30px;
    justify-content: center;
}

@media only screen and (min-width: 768px) {
#galleryLoop {
      grid-template-columns: auto auto;
  }
}

@media only screen and (min-width: 1000px) {
#galleryLoop {
      grid-template-columns: auto auto auto;
  }
}
</style>
