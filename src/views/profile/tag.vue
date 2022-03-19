<template>

    <div class="bot">
      <div class="left-side-bot">
        <div class="media-small">
          <img
            src="https://pbs.twimg.com/media/FFhIRicXoAMvwAd?format=jpg&name=medium"
            alt=""
          />
        </div>
        <div class="media-small">
          <img
            src="https://pbs.twimg.com/media/FFhIR6-XEAMzqD6?format=jpg&name=medium"
            alt=""
          />
        </div>
        <div class="media-small">
          <img
            src="https://pbs.twimg.com/media/FEFXWNJWUAM8BPU?format=jpg&name=medium"
            alt=""
          />
        </div>
      </div>
    </div>
     
 
</template>

<script>
import CustomText from "@/components/CustomText";

export default {
  name: "tag",
  components: {
    CustomText,
  },
};
</script>

<style scoped>
.tag {
  display: grid;
  grid-template-rows: 100px 1fr;
  justify-content: center;
  align-items: center;
}


.tag-text {
  display: inline-flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin-bottom: 50px;
}

.tag-text2 {
  max-width: 350px;
  max-height: 50px;
}

.thin {
  font-weight: 100;
  font-size: 25px;
}

.post {
  background-color: rgb(250,250,250);
}
.post-media{
  display: none;
}
.post-media {
  display: inherit;
  width: 250px;
  height: 293px;
}

.post-media:hover {
  -webkit-filter: brightness(75%);
  -webkit-transition: all ease;
  -moz-transition: all ease;
  -o-transition: all ease;
  -ms-transition: all ease;
  transition: all ease;
}




</style>


 <style scoped>
 
.explore {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  max-width: 930px;
}

.media-small {
  border: 1px solid white;
}

.media-big {
  border: 1px solid white;
}
.top {
  display: grid;
  grid-template-columns: 1fr;
}

.bot {
  display: grid;
  grid-template-columns: 1fr;
}

@media screen and (min-width: 980px) {
  .explore {
    display: flex;
    flex-direction: column;
    width: 930px;
  }

  .top {
    display: grid;
    grid-template-columns: 1fr 2fr;
    column-gap: 30px;
    max-width: 900px;
    max-height: 630px;
  }

  .bot {
    padding-bottom: 30px;
  }

  .right-side-top {
    display: grid;
    grid-template-rows: 1fr;
    max-height: 570px;
  }

  .left-side-top {
    display: grid;
    grid-template-rows: 1fr 2fr;
    row-gap: 30px;
  }

  .left-side-bot {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    column-gap: 30px;
  }

  .media-small {
    display: inherit;
    width: 290x;
    height: 290px;
    cursor: pointer;
    -webkit-filter: brightness(100%);
  }

  .media-small:hover {
    -webkit-filter: brightness(75%);
    -webkit-transition: all ease;
    -moz-transition: all ease;
    -o-transition: all ease;
    -ms-transition: all ease;
    transition: all ease;
  }

  .media-big {
    display: inherit;
    width: 610px;
    height: 600px;
    cursor: pointer;
    -webkit-filter: brightness(100%);
  }

  .media-big:hover {
    -webkit-filter: brightness(75%);
    -webkit-transition: all ease;
    -moz-transition: all ease;
    -o-transition: all ease;
    -ms-transition: all ease;
    transition: all ease;
  }
}

 </style>

