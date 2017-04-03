# Country-Region DropDown Menu
This javascript enables user to easily implement a country-region dropdown menu.
It is as simple as by entering the given attribute into the country and region dropdown menu respectively to make them works.
After that, the region dropdown will be automatically refresh on the change of country dropdown.

## Usage

    <html>
      <head>
        <meta charset="UTF-8">
        <script src="dist/geodatasource-cr.min.js"></script>
      </head>
      <body>

        <div>
            Country: <select class="gds-cr" country-data-region-id="gds-cr-one" ></select>

            Region: <select id="gds-cr-one" ></select>
        </div>

        <div>
            Country: <select class="gds-cr" country-data-region-id="gds-cr-two" country-data-default-value="United States"></select>

            Region: <select id="gds-cr-two" region-data-default-value="California"></select>
        </div>

      </body>
    </html>


## Bootstrap Usage
If you are using Twitter Bootstrap, you may refer to the below example for the implementation.

    <!DOCTYPE html>
    <html>
    <head>
        <meta charset="UTF-8">
        <title>Country-Region DropDown Menu</title>
    
        <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">
        <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap-theme.min.css" integrity="sha384-rHyoN1iRsVXV4nD0JutlnGaslCJuC7uwjduW9SVrLvRYooPp2bWYgmgJQIXwl/Sp" crossorigin="anonymous">
    
        <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js" integrity="sha384-Tc5IQib027qvyjSMfHjOMaLkfuWVxZxUPnCJA7l2mCWNIpG9mGCD8wGNIcPD7Txa" crossorigin="anonymous"></script>
        <script src="dist/geodatasource-cr.min.js"></script>
    </head>
    <body>
        <div class="container">
            <div class="row">
                <div class="col-md-12 text-center" style="margin-bottom:40px;">
                    <h2>Country-Region DropDown Menu</h2>
                </div>
                <div class="col-md-12">
                    <form class="form-horizontal">
                        <div class="form-group">
                            <label class="col-sm-2 control-label">Country</label>
                            <div class="col-sm-10">
                                <select class="form-control gds-cr" country-data-region-id="gds-cr-1"></select>
                            </div>
                        </div>
                        <div class="form-group">
                            <label for="gds-cr-1" class="col-sm-2 control-label">Region</label>
                            <div class="col-sm-10">
                                <select class="form-control" id="gds-cr-1"></select>
                            </div>
                        </div>
                    </form>
                </div>
            </div>
        </div>
    </body>
    </html>


## Node.js Usage
The following steps show how to use the dropdown menu in **Express Web Framework**:

1. Install the module by ```npm install country-region-dropdown-menu```
2. Copy geodatasource-cr.min.js script to ```/public/javascripts/``` directory.
3. Include the script in the jade file by ```script(src='/javascripts/geodatasource-cr.min.js')```
4. Code for implementation:
```
    |Country:
    select.gds-cr(country-data-region-id="gds-cr-one")
    |Region:
    select#gds-cr-one
```

## Attributes

* Country field **must** be given a class name as ```gds-cr``` .
* ```country-data-region-id``` is **required** in country field that contains the id of region field.
* ```country-data-default-value``` is optional in country field which use to set the default selected country value.
* ```region-data-default-value``` is optional in region field which use set the default selected region value. 

## Demo

Please check on [demo](http://www.geodatasource.com/software/country-region-dropdown-menu-demo) page to have a clearer picture about how it works.

## Sample page

Please refer to example.html file.

## Support

Email: support@geodatasource.com  
URL: [http://www.geodatasource.com](http://www.geodatasource.com)
