<template>
  <div>
    <div id="mv">
      <div id="mv-content">
        <div id="icon">
          <img src="../assets/images/icon.png" alt="アイコン">
        </div>
        <img src="../assets/images/copy.png" alt="食べるという、コミュニケーション" id="copy">
        <h2 id="desc">「まち」の食育プロジェクト<br>EATOP</h2>
      </div>
    </div>
    <div id="contents-container">
      <topAbout/>
      <topEvent/>
      <topLogs/>
    </div>
  </div>
</template>

<script>
import topAbout from '@/components/topAbout'
import topEvent from '@/components/topEvent'
import topLogs from '@/components/topLogs'

export default {
  name: 'top',
  components: {
    topAbout: topAbout,
    topEvent: topEvent,
    topLogs: topLogs
  }
}
</script>

<style scoped>
* {
  font-family: 'Nasu';
  font-weight: normal;
  text-align: center;
  margin: 0;
}

#mv {
  height: 500px;
  text-align: center;
  background-image: url(../assets/images/mv.png);
  background-repeat: no-repeat;
  background-position: center center;
  background-size: cover;
}

#mv-content {
    background-color: #fff5f281;
    height: 100%;
    width: 60%;
    min-width: 300px;
    max-width: 800px;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    justify-content: space-around;
}

#icon img {
  height: 130px;
}

#copy {
    object-fit: contain;
    height: 120px;
}

#desc {
    font-weight: normal;
    margin: 20px 0;
    color:  rgba(0, 0, 0, 0.692);
}

topAbout topEvent topLogs {
  height: 790px;
}

@media (min-width: 1400px) {
    #mv {
        height: 700px;
    }
    #icon img {
        height: 180px;
    }
    #copy {
        height: 180px;
    }
}

</style>
