<template>
    <div id="header-container">
        <header>
            <div class="nav-cont container ">
                <div class="header-logo">
                    logo
                </div>
                <ul>
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
</template>

<script>
    export default {
        
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
     flex-direction: column;
     justify-content: space-between;
     align-items: start;
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

  @media screen and (max-width: 576px){
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

  @media screen and (min-width: 992px){
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

  @media screen and (min-width: 1024px){
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