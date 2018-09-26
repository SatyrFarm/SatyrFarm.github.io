If you are creating custom farm items that you wish to share with others, contact us to be added to this list

## Farm regions List

<table id="example" class="display" style="width:100%">
        <thead>
            <tr>
                <th>Title</th>
                <th>Descr</th>
           
            </tr>
        </thead>
        <tfoot>
            <tr>
                <th>Title</th>
                <th>Descr</th>
               
            </tr>
        </tfoot>
    </table>


<script>
 $(document).ready(function() {
    $('#farmtable').DataTable( {
        "ajax": {
            "url": "farms.json",
            "dataSrc": ""
        },
        "columns": [
            { "data": "title" },
            { "data": "descr" }
        ]
    } );
} );
  </script>
