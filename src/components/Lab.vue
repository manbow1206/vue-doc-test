<template>
    <div>
        <h1>{{ propData }}</h1>
        <p>{{ text }}</p>
    </div>
</template>

<script>
export default {
    props: {
        // 基本的な型の検査 (`null` と `undefined` は全てのバリデーションにパスします)
        propA: Number,

        // 複数の型の許容
        propB: [String, Number],

        // 文字列型を必須で要求する
        propC: {
          type: String,
          required: true
        },

        // デフォルト値つきの数値型
        propD: {
          type: Number,
          default: 100
        },

        // デフォルト値つきのオブジェクト型
        propE: {
          type: Object,
          // オブジェクトもしくは配列のデフォルト値は
          // 必ずそれを生み出すための関数を返す必要があります。
          default: function () {
            return { message: 'hello' }
          }
        },

        // カスタマイズしたバリデーション関数
        propF: {
          validator: function (value) {
            // プロパティの値は、必ずいずれかの文字列でなければならない
            return ['success', 'warning', 'danger'].indexOf(value) !== -1
          }
        
        }
      },
    data(){
        return {
            // title: "Header",
            text: "Hello Vue.js!"
        }
    }
}
</script>

<style scoped>
div{
    border: 2px solid teal
}
h1{
    color: teal
}
p{
    color:rgb(27, 77, 77)
}
</style>
