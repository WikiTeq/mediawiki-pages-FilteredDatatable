# Filtered Datatable package

Provides a script to load datatables and a template to add the Search Builder interface to the mediawiki table (SMW).

# Requirements

* SemanticMediaWiki

# Setup

## via PagePort 

* download the repository
* run `php extensions/PagePort/maintenance/importPages.php --source ~/mediawiki-pages-FilteredDatatable`

## via PageExchange

* add the following to the bottom of your `LocalSettings.php`: 
```
$wgPageExchangePackageFiles[] = 'https://raw.githubusercontent.com/WikiTeq/mediawiki-pages-FilteredDatatable/master/page-exchange.json';
```
* navigate to `Special:Packages` and install the package
* (optional) run `php maintenance/runJobs.php`

# Usage

* Navigate to `Project:Datatable` to see the example.
* Read documentation for `Template:Datatable`.
* Create semantic queries and wrap them as described in the documentation.
