<template>
    <div id="header-container">
        <header>
            <div class="nav-cont container">
                <div class="header-logo">
                    logo
                </div>
                <div  class="icon">
                    <i @click="toggleModal" class="bx bx-menu"></i>
                </div>
                <ul v-show="show">
                    <li><a href="#">Home</a></li>
                    <li><a href="#">About</a></li>
                    <li><a href="#">Service</a></li>
                    <li><a href="#">Domain</a></li>
                    <li><a href="#">Command</a></li>
                    <li><a href="#">Contact</a></li>
                </ul>
            </div>
        </header>
    </div>
    
    <div class="container lorem">
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sunt labore ut voluptas officia 
         eveniet animi accusamus voluptatum excepturi! Numquam harum, eveniet temporibus aliquam laudantium pariatur rem libero quas cum accusantium explicabo neque optio sequi consectetur ratione ducimus fugiat id tenetur? Non quidem error itaque ipsam, recusandae nobis quis, ut optio, officiis voluptate earum sequi aut facere sunt excepturi architecto consequuntur sed? Dolorem laboriosam eius, in veritatis ab quis? Sapiente non quam assumenda aut ipsam exercitationem placeat. Minima quasi numquam quisquam voluptatem vel omnis, minus deserunt modi illum suscipit accusantium hic nobis aliquam, totam dolore harum id vitae doloribus. Accusantium totam suscipit recusandae cumque, similique reiciendis! Autem numquam odio non, doloremque minima, expedita nisi cum fugit debitis architecto in ipsa animi, consequatur quasi vitae. Quas itaque accusantium earum architecto autem unde natus at modi, praesentium quo asperiores sit quibusdam sequi optio assumenda blanditiis, ullam nihil consequatur? Non soluta sequi error natus! Explicabo, molestias ex dignissimos architecto sapiente harum officiis quibusdam iste nam est laboriosam molestiae aliquid corporis ratione eveniet soluta numquam illo aperiam ad deserunt error porro sit sint! Exercitationem ipsam doloremque aliquid vel porro culpa velit! Ab voluptatum pariatur tenetur doloremque architecto ipsa possimus quia eaque minus eius, ipsum repellendus!

         <p>
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Hic laborum voluptas consequuntur! Inventore laboriosam quidem ipsum rerum porro doloremque cum! Harum magnam modi corporis optio itaque, doloremque perspiciatis quasi voluptatibus quidem earum commodi velit inventore perferendis quia molestiae ratione? Aspernatur aliquid esse mollitia soluta architecto ea natus maiores suscipit id in! Doloribus unde error reiciendis iusto quia perspiciatis quo repudiandae eaque explicabo? Tempora libero nihil ex ducimus? Excepturi id explicabo labore, totam ducimus iste sit nesciunt cum voluptatem laborum quos repellendus odit provident a necessitatibus, quia consectetur expedita nisi blanditiis non nam? Unde, debitis. Reprehenderit sapiente voluptatibus, eos ipsum ut consectetur est, unde, a ad voluptas ratione hic modi dolorum non asperiores voluptates. Adipisci quidem, dicta nesciunt fuga eaque deleniti odio repudiandae quia error aliquam, vel ullam rem? Unde id, dolorum itaque, quae nobis rem voluptate natus ratione aliquid harum blanditiis consequuntur eveniet at eum dicta mollitia, reprehenderit tempore sapiente dolores molestiae dolor alias temporibus. Rem eveniet, alias assumenda tempore dolorem recusandae ullam ratione quas ea amet itaque magnam ad a illo natus ducimus perferendis consectetur neque voluptatibus ipsum. Ut vitae optio atque sapiente officia nesciunt, architecto blanditiis dolore eos at quaerat veritatis ipsam maiores illo nam nobis praesentium incidunt dolorem pariatur, neque explicabo! Dolorem architecto fugit pariatur alias sapiente? Eligendi cumque esse ad corporis mollitia sed molestiae corrupti aperiam, laudantium eos sequi ipsam voluptates hic id magnam aliquam laborum officiis consequuntur expedita ex ab consectetur repellendus amet iusto. Dignissimos repellat molestiae accusamus provident a! Et incidunt voluptatibus architecto neque distinctio dolores ex dicta, laborum quisquam quasi blanditiis hic molestiae suscipit mollitia earum non tenetur iusto maiores? Quae, sapiente? In eum ipsam nobis at earum veritatis, similique officiis, optio impedit, omnis eveniet eligendi recusandae inventore exercitationem vel ducimus consequatur hic explicabo ipsa animi odio rerum. Ratione ipsum repellat labore voluptas!
         </p>
    </div>
</template>

<script setup>
    import { ref } from 'vue';
    const show = ref(true);

    const toggleModal = () =>{
        show.value = !show.value
    }
</script>

<style scoped>
  #header-container{
      background-color: rgb(241, 69, 241);

  }

  .header-logo{
    font-size: 18px;
    text-transform: capitalize;
    color: black;
    font-weight: bold;
    cursor: pointer;
  }

  .nav-cont{
     display: flex;
     flex-direction: row;
     justify-content: space-between;
     align-items: center;
     position: relative;
     /* padding: 10px; */
  }
    
  
  ul,li{
    list-style-type: none;
    display: flex;
  }

   a{
        padding: 15px;
        font-size: 18px;
        text-decoration: none;
        color: white;
   }

    a:hover{
          background-color: white;
          color: rgb(241, 69, 241);
          width: full;
    }

    .icon i{
        font-size: 40px;
        visibility: hidden;
        /* display: none; */
    }

    .lorem{
        margin-top: 2rem;
    }

  @media screen and (max-width: 576px){
        .nav-cont{
            flex-direction: column;
            justify-content: start;
            align-items: start;
            width: 100%;
            padding: 10px;
        }

        .header-logo{
            width: 100%;
            padding-left: 10px;
        }

        ul{
            position: absolute;
            background-color: rgb(241, 69, 241);
            top: 100%;
        }


        ul,li{
            list-style-type: none;
            flex-direction: column;
            justify-content: start;
            width: 100%;
        }

        a{
            padding: 15px;
            font-size: 18px;
            text-decoration: none;
            color: white;
        }

        a:hover{
            background-color: white;
            color: rgb(241, 69, 241);
            width: full;
        }

        .icon i{
            visibility: visible;
            position: absolute;
            top: 0%;
            right: 5%;
        }

        .lorem{
            padding: 0 10px;
        }
      
  }

  @media screen and (max-width: 992px){
        .nav-cont{
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        ul,li{
            list-style-type: none;
            display: flex;
        }

        a{
            padding: 20px;
            font-size: 18px;
            text-decoration: none;
            color: white;
        }

        a:hover{
            background-color: white;
            color: rgb(241, 69, 241);
            width: full;
        }
  }

    @media screen and (max-width: 1024px){
        .nav-cont{
                display: flex;
                justify-content: space-between;
                align-items: center;
        }

        ul,li{
            list-style-type: none;
            display: flex;
        }

        a{
            padding: 15px;
            font-size: 18px;
            text-decoration: none;
            color: white;
        }

        a:hover{
            background-color: white;
            color: rgb(241, 69, 241);
            width: full;
        }
    }
</style>