<template>
  <div class="post">
    <!-- header -->
    <div class="head section">
      <div class="head-author">
        <div class="head-avatar">
          <img
            src="https://pbs.twimg.com/profile_images/1346076211521449991/CAIzJaNA_400x400.jpg"
            alt="avatar"
            width="40px"
            height="40px"
          />
        </div>

        <div class="head-author-info">
          <div>
            <CustomText tag="b">JobsWire</CustomText>
          </div>
          <div>
            <CustomText size="xsmall">İstanbul</CustomText>
          </div>
        </div>
      </div>
      <div class="head-more">
        <button type="button">
          <IconMore />
        </button>
      </div>
    </div>

    <!-- media -->
    <div class="post-media">
      <img
        src="https://pbs.twimg.com/media/FNUqNIgXoAMQQcb?format=jpg&name=medium"
        alt=""
      />
    </div>

    <!-- actions -->
    <div class="action-buttons section">
      <button type="button">
        <IconLike />
      </button>
      <button type="button">
        <IconComment />
      </button>
      <button type="button">
        <IconDirect />
      </button>
      <button class="action-save" type="button">
        <IconSave />
      </button>
    </div>

    <!-- view count -->

    <div class="view-count section">
      <custom-text tag="b">350 beğenme</custom-text>
    </div>

    <!-- comment list -->
    <div class="view-comment section">
      <custom-text tag="b">JobsWire</custom-text>
      Kadınlar dünya nüfusunun yarısını oluşturuyor olsa da günümüzde hala eşitlik mücadelesi vermek zorunda kalmak canımızı yakıyor. Özellikle de iş dünyasında mobbinge uğrayan, yetenekleri görmezden gelinen pek çok kadın için savaşmaya ve daha eşit bir iş dünyası kurmak için çalışmaya devam ediyoruz. ✔️

JobSwire olarak iş dünyasında cinsiyete değil yetkinliğe ve yeteneklere önem veriyoruz bu nedenle de sizlere kayıt sırasında cinsiyetinizi sormuyoruz ve asla da sormayacağız. Dünyayı değiştirmenin, dünyamızı değiştirmekle başladığına inanıyoruz. 😉

İki kadın kurucu ortağın omuzlarında yükselen JobSwire, canı gönülden tüm kadınların; 8 Mart Dünya Kadınlar Günü’nü kutluyor. Daha eşit ve daha aydınlık yarınlarımızın olması dileğiyle! 💪

Son olarak yana kaydırarak günün öneri filmine de ulaşabilirsin! 😎
    </div>
    <!-- datetime -->
    <div class="view-datetime section">
      <div class="view-datetime text">
        <CustomText tag="b" size="xsmall">2 HOURS AGO</CustomText>
      </div>
    </div>
    <!-- comment form -->
    <div class="comment-form section">
      <button type="button">
        <Emoji />
      </button>
      <form class="comment-form commentline">
        <input type="Text" placeholder="Add a comment..."/>
      </form>
      <button class="action-share" type="button">
        <CustomText tag="b" size="large">Paylaş</CustomText>
      </button>
    </div>

  </div>
  
</template>

<script>
import Avatar from "@/components/Avatar";
import CustomText from "@/components/CustomText";
import IconMore from "@/icons/more.svg";
import IconLike from "@/icons/like.svg";
import IconComment from "@/icons/comment.svg";
import IconDirect from "@/icons/direct.svg";
import IconSave from "@/icons/save.svg";
import Emoji from "@/icons/emoji.svg";

export default {
  name: "Post",
  components: {
    IconLike,
    IconComment,
    IconDirect,
    IconSave,
    IconMore,
    CustomText,
    Avatar,
    Emoji
  },
  data: function () {
    return {
      notPost: false,
    };
  },
};
</script>

<style scoped>
.post {
  border-radius: 3px;
  border: 1px solid rgb(209, 209, 209);
  background-color: white;
  margin-bottom: 62px;
}

.section {
  padding-left: 16px;
  
}

.text {
  color:gray;
}

.head {
  height: 60px;
  display: flex;
  align-items: center;
}

.head-avatar {
  display: inline-flex;
  border-radius: 50%;
  background: linear-gradient(
    219deg,
    rgba(184, 63, 140, 1) 0%,
    rgba(237, 158, 90, 1) 100%
  );
}

.head-avatar img {
  border-radius: 50%;
}

.head-author {
  display: flex;
  align-items: center;
}

.head-author-info {
  margin-left: 8px;
}

.head-more {
  margin-left: auto;
  padding-right: 16px;
}

.action-buttons {
  height: 45px;
  display: flex;
  align-items: center;
}

.action-buttons button {
  margin-right: 16px;
}

.action-save {
  margin-left: auto;
  margin-right: 0;
}

.action-share {
  margin-left: auto;
  margin-right: 0;
  color:#0095f6;
  padding-right: 16px;
}

.post-media {
  min-width: 100px;
  min-height: 100px;
  background-color: rgb(245, 245, 245);
}

.view-comment {
  padding-top: 8px;
}

.comment-form {
  border-top:1px solid rgb(209, 209, 209);
  height: 50px;
  display: flex;
  align-items: center;
  margin-top: 16px;
  overflow:hidden
}

.commentline {
  padding-left: 16px;
  font-weight: 600;
  padding-bottom: 16px;
}

.commentline input {
  width: 540px; 
}

@media screen and (min-width: 980px) {
  .action-share {
  margin-left: auto;
  margin-right: 0;
  color:#0095f6;
  padding-right: 16px;
}

.comment-form {
  border-top:1px solid rgb(209, 209, 209);
  height: 50px;
  display: flex;
  align-items: center;
  margin-top: 16px;
}
}

</style>
