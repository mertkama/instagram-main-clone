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
  
      </div>
    </div>
     
</template>

<script>
import CustomText from "@/components/CustomText";

export default {
  name: "igtv",
  components: {
    CustomText,
  },
};
</script>

<style scoped>
.igtv {
  display: grid;
  grid-template-rows: 100px 1fr 1fr;
  justify-content: center;
  align-items: center;
}

.igtv-icon {
  width: 85px;
  height: 85px;
  display: inline-flex;
  justify-content: center;
  align-items: center;
  padding-left: 110px;
}

.igtv-text {
  display: inline-flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.igtv-upload {
  width: 100px;
  height: 30px;
  padding-left: 105px;
  padding-top: 20px;
}

.action-edit {
  background-color: dodgerblue;
  padding: 0.5rem;
  border-radius: 3px;
  color: white;
  width: 100px;
  height: 30px;
}

.thin {
  font-weight: 100;
  font-size: 25px;
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
