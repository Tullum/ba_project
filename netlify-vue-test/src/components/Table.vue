<template>
    <div id="#table">
    
        <v-data-table
        :headers="headers"
        :items="projects"
        :item-pr-prage="5"
        class="elevation-1"
        ></v-data-table>

        <div class="table">
            <table style="width: 100%">
                <tr>
                    <th>Project</th>
                    <th>Time spend</th>
                    <th>Project status</th>
                    <th>Client connection</th>
                    <th>Add new</th>
                </tr>
                <tr>
                    <td>Stark</td>
                    <td>16 hours</td>
                    <td>Done</td>
                    <td>Bob Bobsen</td>
                    <td>Edit/Delete</td>
                </tr>
                <tr>
                    <td>Jem&Fix</td>
                    <td>10 hours</td>
                    <td>In Progress</td>
                    <td>John Johnson</td>
                    <td>Edit/Delete</td>
                </tr>
                <tr>
                    <td>Bauhaus</td>
                    <td>9 hours</td>
                    <td>Ready to start</td>
                    <td>Marc Marcson</td>
                    <td>Edit/Delete</td>
                </tr>
                <tr>
                    <td>Stark</td>
                    <td>16 hours</td>
                    <td>Done</td>
                    <td>Bob Bobsen</td>
                    <td>Edit/Delete</td>
                </tr>
            </table>        
        </div>

    </div>
</template>

<style>
.table{
   
   border: 1px solid black
}

</style>


<!--<script>
export default {
  name: "TableStructure",
    data(){
        return{
            headers: [
                {
                    text: "Project",
                    align: "left",
                    sortable: false,
                    value: "project",
                },

                {text: "Time spend", value: "hours"},
                {text: "Project status", value: "status"},
                {text: "Client connection", value: "connection"},
            ],
            projects: [
                {
                project: "Stark",
                hours: 10,
                status: "In progress",
                connection: "Bob Bobsen",
                },
            ],
            methods: {
                getColor (status) {
                    if (status = "Start") return "red"
                    else if (status = "In progress") return "orange"
                    else return "green"
                },
            }
        }
    },
};
</script>-->