# Saving-Checkbox-States-Between-Datatables-Pages
Saving Checkbox states between Datatables pages
// DataTable Render

        "columnDefs": [
        {
            "render": function (data, type, row) {
              if (ListChecked.indexOf(row[1]) > -1) {
                  return '  <input type="checkbox" class="filled-in" id="box' + row[0] + '" value="' + row[1] + '" />
              }
              else
              {
                  return '  <input type="checkbox" class="filled-in" id="box' + row[0] + '" value="' + row[1] + '" checked />
              }
          }, "targets": 1  },
          { "visible": false, "targets": [0] }
        ],
