<script>
export default {
    data(){
        return{
            ftarr:[
                {
                    img:'buy-comics-digital-comics.png',
                    tittle:'DIGITAL COMICS',
                },
                {
                    img:'buy-comics-merchandise.png',
                    tittle:'DC MERCHANDISE',
                },
                {
                    img:'buy-comics-subscriptions.png',
                    tittle:'SCUBSCRIPTION',
                },
                {
                    img:'buy-comics-shop-locator.png',
                    tittle:'COMIC SHOP LOCATOR',
                },
                {
                    img:'buy-dc-power-visa.svg',
                    tittle:'DC POWER VISA',
                },
            ]
        }
    },
    methods: {
		getImagePath(img) {
			return new URL(`../assets/img/${img}`, import.meta.url).href;
		},
	},
}
</script>
<template >

    <div class="top-foot">
        <div class="max-w">
            <div class="features-ft"
            v-for="obj in ftarr" 
            >
                <img :src="getImagePath(obj.img)" alt="">
                <span>{{ obj.tittle }}</span>
            </div>
        </div>
    </div>
    <div class="main-foot">
        <div class="max-w">
            <div class="sub-cont">
                <div class="col">
                    <ul>
                        <li>DC COMICS</li>
                        <li>Comics</li>
                        <li>Comics</li>
                        <li>Comics</li>
                        <li>Comics</li>
                        <li>Comics</li>
                        <li>Comics</li>
                    </ul>
                    <ul>
                        <li>DC COMICS</li>
                        <li>Comics</li>
                        <li>Comics</li>
                    </ul>
                </div>
                <div class="col">
                    <ul>
                        <li>DC COMICS</li>
                        <li>Comics</li>
                        <li>Comics</li>
                        <li>Comics</li>
                        <li>Comics</li>
                        <li>Comics</li>
                        <li>Comics</li>
                        <li>Comics</li>
                        <li>Comics</li>
                    </ul>
                </div>
                <div class="col">
                    <ul>
                        <li>DC COMICS</li>
                        <li>Comics</li>
                        <li>Comics</li>
                        <li>Comics</li>
                        <li>Comics</li>
                    </ul>
                </div>
            </div>
            <img src="../assets/img/dc-logo-bg.png" alt="">
        </div>
    </div>
    <div class="bottom-foot">
        <div class="max-w"></div>
    </div>

</template>


<style lang="scss" scoped>
@use './../assets/styles/partials/variable' as *;

    .top-foot{
        background-color: $bg-tf ;
        padding: 2rem;
        display: flex;
        justify-content: center;
        gap: 1rem;
        color: white;
        .features-ft{
            display: flex;
            justify-content: center;
            align-items: center;
            gap: .5em;
            span{
                white-space: nowrap;
            }
            img{
                height: 45px;
                max-width: 45px;
            }
        }
    }
    .main-foot{
        color: white;
        background-image: url('../assets/img/footer-bg.jpg');
        padding: 3rem;
        
        position: relative;
        img{
            max-width: 45%;
            position: absolute;
            top: -25%;
            right: 0;
        }
        .sub-cont{
            display: flex;
            gap: 1rem;
            ul{
                display: flex;
                flex-direction: column;
                gap: .3em;
                margin-bottom: .3em;
            }
        }
    }
    .bottom-foot{
        background: $bg-fb;
        height: 70px;
        position: relative;
        top: 0;
    }
</style>