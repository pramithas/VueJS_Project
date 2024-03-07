<template>
<h1>Props in Vue js 3</h1>
<Student :name="studentName" />
<Teacher :name="teacherName" />
</template>

<script>
import Student from './Student.vue';
import Teacher from './Teacher.vue';

export default {
    name: "Home",

    data() {
        return {
            studentName: "Pramithas Dhakal",
            teacherName: "Devan Gurung"
        }
    },

    components: {
        Student,
        Teacher
    }
}
</script>

<style>

</style>
