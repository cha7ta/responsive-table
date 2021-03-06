# responsive-table
Responsive table for Desktop and mobile devices
### Styles
```
 <style>      
        /* = Scroll body
    ------------------------*/
        ::-webkit-scrollbar {
            width: 0.2em;
        }

        ::-webkit-scrollbar-track {
            background-color: #bdc3c7;
        }

        ::-webkit-scrollbar-thumb {
            background-color: #7f8c8d;
        }

        /* = table
    ------------------------*/
        .box-table table {
            border-collapse: collapse;
            position: relative;
            height: 300px;
            width: 100%;
            overflow-y: auto;
            overflow-x: hidden;
        }

        thead,
        tbody,
        tbody tr {
            display: table;
            width: 100%;
            table-layout: fixed;
        }

        thead {
            position: absolute;
            top: 0;
            z-index: 10;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        tbody {
            display: block;
            height: 100%;
            overflow-y: auto;
            position: absolute;
            box-sizing: border-box;
        }

        .box-table table {
            border-collapse: collapse;
            text-align: left;
            width: 100%;
            margin: 0;
            padding: 0;
            background: #7f8c8d;
            animation: responsive 5s infinite ease-in-out;
        }

        .box-table {
            font: normal 12px/150% Arial, Helvetica, sans-serif;
            overflow: hidden;
            margin: 0 auto;
            display: block;
            width: 95%;
            padding: 2.5%;
        }

        .box-table table thead th {
            background-color: #7f8c8d;
            color: #bdc3c7;
            text-align: center;
            padding: 1em;
            font-family: 'Vollkorn', serif;
            font-weight: bold;
            vertical-align: top;
            border-left: 0.25em double #95a5a6;

        }

        .box-table table tbody td {
            font-family: 'Vollkorn', serif;
            font-size: 1em;
            border: none;
            padding: 1em;
        }

        .box-table table tbody tr:nth-child(odd) {
            background: #ecf0f1;
            color: #95a5a6;
        }

        .box-table table tbody tr:nth-child(even) {
            background: #bdc3c7;
            color: #7f8c8d;
        }

        .box-table table tbody tr a {
            text-decoration: none;
            color: #e67e22;
        }

        .box-table table tbody tr a:hover {
            color: #d35400;
        }

        .box-table .user-photo {
            background: #bdc3c7;
        }

        .box-table .user-tumb {
            width: 6em;
            height: 6em;
            padding: 0;
            display: table-cell;
            text-align: center;
            margin: 0 auto;
            -webkit-border-radius: 100%;
            -moz-border-radius: 100%;
            border-radius: 100%;
        }


        /* = Responsive table
    ------------------------*/

        /* http://elvery.net/demo/responsive-tables/  */
        @media only screen and (max-width: 800px) {
            .box-table table {
                width: 100%;
                border-collapse: collapse;
                border-spacing: 0;
            }

            thead,
            tbody,
            tbody tr {
                width: auto;
            }

            .box-table th,
            .box-table td {
                margin: 0;
                vertical-align: top;
            }

            .box-table th {
                text-align: left;
            }

            .box-table table {
                display: block;
                position: relative;
                width: 100%;
                height: auto;
            }

            .box-table thead {
                display: block;
                float: left;
                position: inherit;
            }

            .box-table tbody {
                display: block;
                width: auto !important;
                position: relative;
                overflow-x: auto;
                white-space: nowrap;
            }

            .box-table thead tr {
                display: block;
            }

            .box-table th {
                display: block;
                text-align: right;
            }

            .box-table tbody tr {
                display: inline-block;
                vertical-align: top;
            }

            .box-table td {
                display: block;
                min-height: 1.25em;
                text-align: left;
            }

            .box-table th {
                border-bottom: 0;
                border-left: 0;
            }

            .box-table td {
                border-left: 0;
                border-right: 0;
                border-bottom: 0;
            }
        }
    </style>
```
#### HTML Code
```html
<!DOCTYPE html>
<html>
    <head>
        <mate charest="utf-8" />
        <title>Hello world!</title>
    </head>
   <body>
    <!-- Description -->
    <h1 class="description">
        Responsive Table
    </h1>
    <!-- Table demo -->
    <div class="box-table">
        <table class="table table-striped">
            <thead>
                <tr>
                    <th>Firstname</th>
                    <th>Middle Name</th>
                    <th>Lastname</th>
                    <th>Email</th>
                    <th>Phone Num</th>
                    <th>Addess</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>Abdul</td>
                    <td>Rahman</td>
                    <td>R</td>
                    <td>abc@gmail.com</td>
                    <td>123456789</td>
                    <td>Hyderabad</td>
                </tr>
                <tr>
                    <td>Abdul</td>
                    <td>Rahman</td>
                    <td>R</td>
                    <td>abc@gmail.com</td>
                    <td>123456789</td>
                    <td>Hyderabad</td>
                </tr>
                <tr>
                    <td>Abdul</td>
                    <td>Rahman</td>
                    <td>R</td>
                    <td>abc@gmail.com</td>
                    <td>123456789</td>
                    <td>Hyderabad</td>
                </tr>
                <tr>
                    <td>Abdul</td>
                    <td>Rahman</td>
                    <td>R</td>
                    <td>abc@gmail.com</td>
                    <td>123456789</td>
                    <td>Hyderabad</td>
                </tr>
                <tr>
                    <td>Abdul</td>
                    <td>Rahman</td>
                    <td>R</td>
                    <td>abc@gmail.com</td>
                    <td>123456789</td>
                    <td>Hyderabad</td>
                </tr>
                <tr>
                    <td>Abdul</td>
                    <td>Rahman</td>
                    <td>R</td>
                    <td>abc@gmail.com</td>
                    <td>8099177174</td>
                    <td>Hyderabad</td>
                </tr>
                <tr>
                    <td>Abdul</td>
                    <td>Rahman</td>
                    <td>R</td>
                    <td>abc@gmail.com</td>
                    <td>123456789</td>
                    <td>Hyderabad</td>
                </tr>
                <tr>
                    <td>Abdul</td>
                    <td>Rahman</td>
                    <td>R</td>
                    <td>abc@gmail.com</td>
                    <td>123456789</td>
                    <td>Hyderabad</td>
                </tr>
                <tr>
                    <td>Abdul</td>
                    <td>Rahman</td>
                    <td>R</td>
                    <td>abc@gmail.com</td>
                    <td>123456789</td>
                    <td>Hyderabad</td>
                </tr>

            </tbody>
        </table>
    </div>

</body>
</html>
```
