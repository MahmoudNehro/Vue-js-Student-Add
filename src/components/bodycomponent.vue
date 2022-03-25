<template>
<addcomponent @newStudentAdded="testeventRaised"/>
    <table class="table table-bordered table-striped">
        <thead>
             <tr>
            <th>Id</th>
            <th>Name</th>
            <th>City</th>
        </tr>
        </thead>
        <tbody>
            <tr v-for="student in students" :key="student.id">
                <td>{{student.id}}</td>
                <td>{{student.name}}</td>
                <td>{{student.city}}</td>
            </tr>
        </tbody>
        <tfoot>
            <tr>
                <th colspan="3">Total Number of Students: {{ students.length }} </th>
            </tr>
        </tfoot>
       
    </table>
</template>
<script>
    import students from '../student'
    import addcomponent from './addcomponent.vue'
    export default {
        data() {
            return {
                students:students
            }
        },
        methods: {
            testeventRaised(data) {
                // console.log("hello from event raised");
                this.students.push(data);
            }

        },
        components:{
        addcomponent
        },

    }
</script>