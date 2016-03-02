# commercial_invoice

foreach($order['shipments'] as $forms)  {
$countlabels++; 
	foreach($forms->forms as $formss)  {
		update_post_meta($order_id, 'easypost_shipping_label_commercial_' . $countlabels, $formss->form_url); 
echo  '<a href="'. $formss->form_url .'">CUSTOMS FORMS</a>';
	}
}
