<template>
<!--    只允许有一个根节点-->
    <div>
        <table>
            <tr>
                <td>编号</td>
                <td>图书名称</td>
                <td>作者</td>
            </tr>
            <tr v-for="item in books">
                <td>{{item.id}}</td>
                <td>{{item.author}}</td>
                <td>{{item.name}}</td>
            </tr>
        </table>
        {{msg}}
    </div>
</template>

<script>
    export default {
        name: "Book.vue",
        data(){
            return{
                msg:"Hello Vue",
                books:[
                    {
                        id: 1,
                        name: "Java零基础实战",
                        author: "xuan1"
                    },
                    {
                        id: 2,
                        name: "Vue零基础实战",
                        author: "xuan2"
                    },
                ]
            }
        }
    }
</script>

<style scoped>

</style>
