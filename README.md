# ajaxPlugin

jQuery plugin like datatables


```
$('table').ajaxGrid({
        requestType: 'get',
        pageSize: 10,
        defaultSortExpression: 'gid',
        defaultSortOrder: 'desc',
        tableHeading: '.table-header',
        url: 'Paginate-AjaxGrid/app/api.php',
        loadingImage: $('#loading-msg'),
        NoRecordsFound: 'No Records Found',
        id: 'gid',
        rowClass: {class: " my-class"},
        addClassToTd: {fields: ['gemail', 'gname'], class: "my-td"}
    });

```
# refresh grid
```
 $('table').trigger("refreshGrid", {filter: document.searchform.filter.value});

```
