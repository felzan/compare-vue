<template>
  <div class="home">
    <section class="hero">
      <div class="hero-body">
        <div class="container">
          <h1 class="title">
            {{ heading }}
            <div class="is-two-thirds column is-paddingless">
              <h2 class="subtitle is-4">
                {{ subheading }}
              </h2>
            </div>
            <a href="" class="button is-large is-primary" id="learn">
              Learn more
            </a>
          </h1>
        </div>
      </div>
    </section>
    
    <section class="section">
      <div class="containet">
        <div class="columns pd is-desktop">
          <div class="columns is-1 has-text-centered">
            <i class="fa fa-cog is-primary"></i>
          </div>
          <div class="columns is-one-third-desktop">
            <p class="title"><strong>Maxime doloremque omnis.</strong></p>
          </div>
          <div class="columns is-one-third-desktop">
            <p>Veritatis nesciunt necessitatibus doloribus tempore. Magni sint dolores est voluptatem est quisquam dolor quaerat inventore. Saepe et impedit et a sit earum et consequatur ut. Sit placeat et assumenda similique aut doloribus. Nobis nihil autem quibusdam. Veniam impedit magni laudantium ad iste.</p>
          </div>
        </div>
      </div>

      <div class="columns pd">
        <div class="column">
           <div class="card">
             <div class="card-content">
               <p class="title">Eaque laborum dolores.Eaque laborum dolores.Eaque laborum dolores.</p>
               <p class="subtitle">Gary Simon</p>
             </div>
           </div>
        </div>
        <div class="column">
           <div class="card">
             <div class="card-content">
               <p class="title">necessitatibus consequatur qui</p>
               <p class="subtitle">Gary Simon</p>
             </div>
           </div>
        </div>
        <div class="column">
           <div class="card">
             <div class="card-content">
               <p class="title">necessitatibus consequatur qui</p>
               <p class="subtitle">Gary Simon</p>
             </div>
           </div>
        </div>
      </div>

    </section>
  </div>
</template>

<script>
export default {
  name: 'home',
  data() {
    return {
      heading: 'Soaring to new heights',
      subheading: 'Inventore vel aut dolor eos amet aperiam molestiae. Maxime et sit eius laborum. Dolores labore culpa quia aut voluptatem dolores a blanditiis alias.'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="sass" scoped>
@import '../mq'

.hero
  background-color: #e3e3e3
  background-size: cover
  
  .title
    +mobile
      fint-wieght: bold
    +tablet
      font-size: 2.5rem
    +desktop
      font-size: 4rem
      margin-top: 2.5rem

h2
  margin: 1.5rem 0 2rem 0 !important

.fa-cog
  font-size: 40px

#learn
  +desktop
    margin-bottom: 2rem
</style>
