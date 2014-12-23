django-js-libs-integration
==========================

Django applications to ease javascript libraries integration in django projects

As of now I included these javascript libraries (maybe some more, if I forget to update README.md):

* jQuery (https://github.com/jquery/jquery)
* Bootstrap (https://github.com/twbs/bootstrap)
* Bootstrap DateTimePicker (https://github.com/Eonasdan/bootstrap-datetimepicker)
* Bootstrap WYSIWYG (https://github.com/bootstrap-wysiwyg/bootstrap3-wysiwyg)
* Moment (https://github.com/moment/moment/)
* Select2 (https://github.com/ivaynberg/select2)
* Datatables (https://github.com/DataTables/DataTables)
* Flot (https://github.com/flot/flot)
* jQplot (https://bitbucket.org/cleonello/jqplot/wiki/Home)

When possible, I chose to use the last stable versions downloaded from the official websites. When this is not possible, I download the last tagged release on the code repository.

The repository tree is organized in this way: first the library, and in every library directory there can be different subdirectories.
Each subdirectory is a Django application named like "library-version", and you hopefully will be able to use it "as is" (suggestions, patches, pull requests are welcome!).

I included the licenses for each library in its main directory.

For now there is no code to check for application dependencies (for example, bootstrap needs jquery, bootstrap datetimepicker needs moment and bootstrap, and so it needs also jquery, and so on...),
and I don't have too much ideas to solve this problem (yes, when you use few plugins you can keep track of dependencies by yourself).
