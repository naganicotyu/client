<template>
    <div>
        <div class="mx-auto grid grid-cols-2 lg:grid-cols-3 p-1 m-1 w-3/4">
        <div  v-for="card in cards" :key="card.title" class="shadow-md border border-gray-50 p-1 m-1 h-40">
        <a href="#" class="grid-item col-span-1  hover overflow-hidden shadow-lg max-w-sm text-gray-600" >
        
            
            <h5 class="text-sm font-semibold p-2 border border-blue-400 text-gray-50 bg-blue-600" >{{card.title}}</h5>
        
        
            <p class="text-xs font-normal text-gray-50 p-2 ">{{card.primary}}</p>
    
    
        </a>
    </div>
    </div>
</div>

    
    </template>
    
    <script>
    export default{
        auth:false,
        data(){
            return{
                cards:[
                {title:"プロフィール",primary:"わたしについて。"},
                {title:"twitter",primary:"twitterです。"},
                {title:"絵",primary:"これは絵です"},
                {title:"スケジュール",primary:"これからのスケジュールｼﾞｭﾙ"},
                {title:"紺です。",primary:"紺のホームページです。"},
                {title:"音楽",primary:"世界は音から始まった"},
                {title:"note",primary:"過去の記事です。"},
                {title:"近頃のあれこれ",primary:"当サイトで色々報告予定です。"},
                {title:"リンク",primary:"様々なリンク集です"},
                ]
            }
        }
    
    
    }
    </script>