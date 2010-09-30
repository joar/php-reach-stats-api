# PHP Halo: Reach Stats API

This is a wrapper for the Halo: Reach SOAP API located at
<http://www.bungie.net/api/reach/ReachApiSoap.svc>.

It has been automatically generated using the service at
<http://apigenerator.com/>

To use this API you must abide by the [Bungie.net API Terms and Conditions][api_tac]

## Usage

Full API documentation is available at [haloreachapi.net][haloreachapi] 

Usage example of the `reachStatsApi`->[GetPlayerDetailsWithStatsByPlaylist][GetPlayerDetailsWithStatsByPlaylist]():

	$api = new reachStatsApi;
	
	$soapResultA = $api->GetPlayerDetailsWithStatsByPlaylist(array(
		'identifier' => $your_api_key,
		'gamertag' => $the_gamertag
	));
	
	var_dump( $soapResultA );
	
	/*
	 * I have no Reach API key, Bungie removed it and told me to 
	 * go pro and I'm not near my Xbox ATM, feel my bitterness.
	 * 
	 * Anyway, I hope that there will be som useful information in
	 * that $soapResultA variable. 
     */

  [api_tac]: http://www.haloreachapi.net/wiki/API_terms_and_conditions
  [GetPlayerDetailsWithStatsByPlaylist]: http://www.haloreachapi.net/wiki/Official_stats_API_documentation#GetPlayerDetailsWithStatsByPlaylist.28System.String.2C_System.String.29
  [haloreachapi]: http://www.haloreachapi.net/wiki/Official_stats_API_documentation