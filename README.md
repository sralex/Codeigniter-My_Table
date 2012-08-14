Codeigniter-My_Table
====================

Extend of core codeigniter library Table.php to add support for tfoot.

#Installation:
Place MY_Table.php in your codeigniter application/libraries folder. *Name and case is important!*

#Usage:

Add a row which is surrounded by tfoot tags.

    $this->table->set_footer('col1','col2','col3');

produces:

    <tfoot>
    <tr>
    <th>col1</th><th>col2</th><th>col3</th>
    </tr>
    </tfoot>

##You can also set the elements used in the template.

    $tmpl = array (
	    'footer_row_start'   => '<tr>',
	    'footer_row_end'     => '</tr>',
    	'footer_cell_start'  => '<th>',
	    'footer_cell_end'    => '</th>'
    )

####Code for this was based on code from https://github.com/EllisLab/CodeIgniter/wiki/Table and modified to work with CodeIgniter 2.1.2, and made into an MY_ extension of the core Table library.
