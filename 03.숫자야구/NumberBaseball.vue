<template> <!-- wordrelay에서 18-27줄-->
    <div>
        <div>{{ result }}</div>
        <form v-on:submit="onSubmitForm">
            <input type="text" ref="answer" v-model="value">
            <button type="submit">입력</button>
        </form>
        <div>시도: {{  }}</div>
    </div>
</template>

<script> // wordrelay에서 17줄
    export default {
        data() {
            return {
                    result: '',
                    value: '',
                }
        },
        methods: {
            onSubmitForm(e) {
                    e.preventDefault();
                },
        },
    };
</script>