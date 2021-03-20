<template>
    <div>
        <v-app-bar absolute elevate-on-scroll　height="75px" id="navbar">
            <v-row>
                <v-col cols="4">
                    <v-row class="title-area">
                        <img src="../assets/winlog.png" height="35px" width="50px" alt="titlelogo">
                        <p  class="discription">Create a field where one can
                        <br>identify a life's passion.
                        </p>
                    </v-row>
                </v-col>

                <v-col cols="6">
                    <nav class="nav">
                        <ul>
                            <li><img src="../assets/train.svg" height="40" width="40" alt="train"></li>
                            <li height="15" width="22.83"><router-link to="#">TOP</router-link></li>
                            <li height="15" width="22.83"><router-link to="#">COMPANY</router-link></li>
                            <li height="15" width="22.83"><router-link to="#">SERVICE</router-link></li>
                            <li height="15" width="22.83"><router-link to="#">NEWS</router-link></li>
                            <li height="15" width="22.83"><router-link to="#">SUPPORTER</router-link></li>
                            <li height="15" width="22.83"><router-link to="#">RECRUIT</router-link></li>
                            <li class="icons"><font-awesome-icon id="twittericon" :icon="['fab', 'twitter']"/></li>
                            <li><font-awesome-icon id="fileicon" :icon="['far', 'file']"/></li>
                        </ul>
                    </nav>
                </v-col>
            </v-row>
        </v-app-bar>
    </div>
</template>

<script>

export default {
}
</script>

<style scoped>
#navbar{
    background: rgba(45,45,45, 0.3);
}
#twittericon{
    color:white;
}
#fileicon{
    transform: scale(-1, 1);
    color:white;
}
.icons{
    display: inline-block;
}

.title-area .discription{
    margin-top: 5px;
    margin-left: 20px;
    color: #fff;
}
.nav{
    /* float: right; */
}
.nav ul{
    display:flex;
}
.nav ul li{
    list-style: none;
    display: inline-block;
    width: 15%; 
    /* ここで項目の幅を指定します */
}
.nav ul li a{
    text-decoration: none;
    color: #333;
}
</style>