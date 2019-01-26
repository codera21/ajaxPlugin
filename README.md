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
### example 
```
 postContent: [

                {
                    control: $('<button  name ="EditPost" type="button" class="btn btn-rounded btn-info" onclick=\'showEditForm(this,"Edit Post","http://kalakathmandu.com/admin/GalleryItem/Form",600,450)\'>' +
                            '<small class="glyphicon glyphicon-pencil"></small>' +
                            ' Edit' +
                            '</button>')
                }

                , {
                    control: $("<form style='display: inline-block' action='http://kalakathmandu.com/admin/GalleryItem/Delete' method='POST'>" +
                            "<input type='hidden' name='ID' id='ID' /> " +
                            '<button name="DeleteUser" type="submit" class="btn btn-rounded btn-danger" onclick=\'return Confirmation(this,"Delete Post","Are you sure you want to delete?", "Yes", "No")\'>' +
                            '<small class="glyphicon glyphicon-trash"></small>' +
                            ' Delete' +
                            '</button></form>'),
                    properties: [
                        {
                            propertyField: 'input[type=hidden]#ID',
                            property: 'value',
                            propertyValue: 'ID'
                        }
                    ]
                }

            ]

```
