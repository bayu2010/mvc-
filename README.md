mvc-
====

library

<div class ='Publishers Index'>
  <h2> Publishers List </h2>
	<table cellpadding = "0">
		<tr>
			<th> <?php echo $this->Paginator->sort('id');
				?> </th>
			<th> <?php echo $this->Paginator->sort('name');
				?> </th>
			<th> <?php echo $this->Paginator->sort('created');
				?> </th>
			<th> <?php echo $this->Paginator->sort('modified');
				?> </th>
		</tr>
		<?php
			$i=0;
			foreach($publishers as $publisher){
				$class = null;
				if ($i++ % 2 == 0) {
					$class ='class ="altrow"';
				}
				?>
			<tr <?php echo $class; ?>>
				<td> <?php echo $publisher['Publisher']['id'];?> </td>
				<td> <?php echo $publisher['Publisher']['name'];?> </td>
				<td> <?php echo $publisher['Publisher']['created'];?> </td>
				<td> <?php echo $publisher['Publisher']['modified'];?> </td>
			</tr>
			<?php } ?>
		</table>
	</div>