# Pagination-Using-JQuery-dataTable-in-Liferay

Imports rquired for pagination :- 

<script src="//ajax.googleapis.com/ajax/libs/jquery/1.11.0/jquery.min.js"></script>
<script type="text/javascript" src="http://cdn.datatables.net/1.10.2/js/jquery.dataTables.min.js"></script>

<script type="text/javascript" src="http://cdn.datatables.net/plug-ins/725b2a2115b/integration/bootstrap/2/dataTables.bootstrap.js"></script>

Html Code :-

<table class="table table-striped error" id="viewDataTables">
 <thead>
  <tr>
   <th><liferay-ui:message key="no" /></th>
   <th><liferay-ui:message key="name" /></th>
  </tr>
 </thead>

        <tbody>
                <tr>
   <td><liferay-ui:message key="123" /></td>
   <td><liferay-ui:message key="Imthiyaz" /></td>
  </tr>
        </tbody>
 </table>

Note :- Here <thead> , <tbody> declaration is mandatory without these pagination will not work .

Script Code :- 

 <script type="text/javascript">

 $('#viewDataTables').dataTable({
     "bFilter" : false,
        "bLengthChange" : false,
        "iDisplayLength" : 10,
        "bSort" : true,
        "sDom" : 't <p> <"bottom"><"clear">'
    
});

 </script>  
