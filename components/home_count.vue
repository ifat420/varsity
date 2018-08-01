<template>
    <div class="container-fluid count">
        <div class="row">
            <div class="col-4 text-left">
                <span class="cheading">
                    <span class="cheading--main count__heading">
                        <strong>JUST</strong>   <br> at a glance
                    </span>
                </span>
            </div>
        </div>
        <div class="row ">
            <div class="col" v-for="(n, i) in count" :key="i">
                <div class="count__item">
                    <div class="count__item--number">
                        {{ n.number }}
                    </div>
                    <div class="count__item--text">
                        {{ n.text }}
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            count: [
                {
                    number: '35',
                    text: 'acres total area'
                },
                {
                    number: '4,234',
                    text: 'total students'
                },
                {
                    number: '206',
                    text: 'faculty members'
                },
                {
                    number: '22',
                    text: 'departments'
                },
                {
                    number: '7',
                    text: 'faculties'
                },
                {
                    number: '2',
                    text: 'total halls'
                }
            ]
        }
    }
}
</script>
