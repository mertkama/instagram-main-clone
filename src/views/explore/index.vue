<template>
  <div class="explore">
    <div class="top">
      <div class="left-side-top">
        <div class="media-small">
          <img
            src="https://pbs.twimg.com/media/FDrwx2NXoAUfELV?format=jpg&name=medium"
            alt=""
          />
        </div>
        <div class="media-small">
          <img
            src="https://pbs.twimg.com/media/FNUqNzHXsAQoAk9?format=jpg&name=medium"
            alt=""
          />
        </div>
      </div>
      <div class="right-side-top">
        <div class="media-big">
          <img
            src="https://pbs.twimg.com/media/FNUqNIgXoAMQQcb?format=jpg&name=medium"
            alt=""
          />
        </div>
      </div>
    </div>
    <div class="bot">
      <div class="left-side-bot">
        <div class="media-small">
          <img
            src="https://pbs.twimg.com/media/FFhIT9pWUAgiRYS?format=jpg&name=medium"
            alt=""
          />
        </div>
        <div class="media-small">
          <img
            src="https://pbs.twimg.com/media/FFhIUbxX0AMJ82I?format=jpg&name=medium"
            alt=""
          />
        </div>
        <div class="media-small">
          <img
            src="https://pbs.twimg.com/media/FFhIU3cXIAUJu_A?format=jpg&name=medium"
            alt=""
          />
        </div>
      </div>
    </div>
    <div class="bot">
      <div class="left-side-bot">
        <div class="media-small">
          <img
            src="https://pbs.twimg.com/media/FFhISjxWYAEZwac?format=jpg&name=medium"
            alt=""
          />
        </div>
        <div class="media-small">
          <img
            src="https://pbs.twimg.com/media/FFhIS_DWQAQ6A30?format=jpg&name=medium"
            alt=""
          />
        </div>
        <div class="media-small">
          <img
            src="https://pbs.twimg.com/media/FFhITYbXEAg2_-c?format=jpg&name=medium"
            alt=""
          />
        </div>
      </div>
    </div>
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
        <div class="bot">
      <div class="left-side-bot">
        <div class="media-small">
          <img
            src="https://pbs.twimg.com/media/FEFXfOTWQAMharh?format=jpg&name=medium"
            alt=""
          />
        </div>
        <div class="media-small">
          <img
            src="https://pbs.twimg.com/media/FEFXftaX0AEneBU?format=jpg&name=medium"
            alt=""
          />
        </div>
        <div class="media-small">
          <img
            src="https://pbs.twimg.com/media/Ev9IzooWEAASigF?format=jpg&name=4096x4096"
            alt=""
          />
        </div>
      </div>
    </div>
        <div class="bot">
      <div class="left-side-bot">
        <div class="media-small">
          <img
            src="https://i.ibb.co/cQnXBGM/r3.jpg"
            alt=""
          />
        </div>
        <div class="media-small">
          <img
            src="https://i.ibb.co/dDzD09D/r2.jpg"
            alt=""
          />
        </div>
        <div class="media-small">
          <img
            src="https://i.ibb.co/QXpsbkR/r1.jpg"
            alt=""
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

import CustomText from "@/components/CustomText";

export default {
  name: "index",
  components: {
    CustomText,
  },
};
</script>

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
    width: 290px;
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
