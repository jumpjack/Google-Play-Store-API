Google-Play-Store-API
=====================


------- Original README -------

## DEPRECATED

Play Store API is an unofficial version of Google Play Store which will let you pullup applications from google play store using18 different functions covering almost everything from google store

<h4> Requirements </h4>
<ol>
  <li> Php 5.0 or greater</li>
	<li> <a href="http://php.net/manual/en/book.curl.php" title="CURL" target="_blank"> CURL </a> enabled server </li>
	<li> Support for <a href="http://php.net/manual/en/function.mb-eregi.php" target="_blank" title="mb_eregi"> mb_eregi </a> function. </li>
</ol>

<h4> Error Handling </h4>
<p> Class itself does all required error handling. All functions will return <strong>0</strong> in case of any error and will return array of data in case of success.</p>

<h4> List Of Functions </h4>
<ol>
	<li><a href="#topPaidApps" title="Top Paid Apps"> Getting Top Paid Apps </a></li>
	<li><a href="#topFreeApps" title="Top Free Apps"> Getting Top Free Apps</a></li>
	<li><a href="#topGrossingApps" title="Top Grossing Apps"> Getting Top Grossing Apps</a></li>
	<li><a href="#topNewPaidApps" title="Top New Paid Apps"> Getting Top New Paid Apps</a></li>
	<li><a href="#topNewFreeApps" title="Top Free Apps"> Getting Top New Free Apps</a></li>
	<li><a href="#topPaidGames" title="Top Paid Games"> Getting Top Paid Games</a></li>
	<li><a href="#topFreeGames" title="Top Free Games"> Getting Top Free Games</a></li>
	<li><a href="#topTrendingApps" title="Getting Trending Apps"> Getting Trending Apps </a></li>
	<li><a href="#staffPicks" title="Getting Staff Picks" target="_blank"> Getting Staff Picks </a></li>
	<li><a href="#staffPicksForTablet" title="Getting Staff Picks For Tablet"> Getting Staff Picks For Tablet </a></li>
	<li><a href="#listCategories" title="List Categories"> List All Categories</a></li>
	<li><a href="#categoryPaidItems" title="Finding Paid Category Items"> Finding Paid Items In A Category </a></li>
	<li><a href="#categoryFreeItems" title="Finding Free Items In A Category"> Finding Free Items In A Category </a></li>
	<li><a href="#developerItems" title="Finding Items From A Certain Developer"> Finding Items From A Certain Developer </a></li>
	<li><a href="#searchStore" title="Search Items"> Search Items </a></li>
	<li><a href="#itemInfo" title="Getting Item Info"> Getting Item Info </a></li>
	<li><a href="#relatedViewed" title="Finding Related Viewed Items"> Finding Related Viewed Items </a></li>
	<li><a href="#relatedInstalled" title="Finding Related Installed"> Finding Related Installed </a></li>
</ol>

<div id="topPaidApps">
	<h4> Getting Top Paid Apps </h4>
	
	<pre class="brush:php">
		include_once('api/playStoreApi.php'); // including class file
		$class_init = new PlayStoreApi;	// initiating class
		
		/* WITHOUT PARAMERTER */
		$topPaidApps = $class_init->topPaidApps(); // calling topPaidApps

		/* PAGINATION PARAMETER */
		// You can easily add the page numbers to paginate the result
		$page = 2;
		$topPaidApps = $class_init->topPaidApps($page); // calling topPaidApps

		if($topPaidApps !== 0)
		{
			print_r($topPaidApps); // it will show all data inside an array
		}
	</pre>
</div>

<div id="topFreeApps">
	<h4> Getting Top Free Apps </h4>
	<pre class="brush:php">
		include_once('api/playStoreApi.php'); // including class file
		$class_init = new PlayStoreApi;	// initiating class

		/* WITHOUT PARAMERTER */
		$topFreeApps = $class_init->topFreeApps(); // calling topFreeApps

		/* PAGINATION PARAMETER */
		// You can easily add the page numbers to paginate the result
		$page = 2;
		$topFreeApps = $class_init->topFreeApps($page); // calling topFreeApps

		if($topFreeApps !== 0)
		{
			print_r($topFreeApps); // it will show all data inside an array
		}
	</pre>
</div>

<div id="topGrossingApps">
	<h4> Getting Top Grossing Apps </h4>
	<pre class="brush:php">
		include_once('api/playStoreApi.php'); // including class file
		$class_init = new PlayStoreApi;	// initiating class

		/* WITHOUT PARAMERTER */
		$topGrossingApps = $class_init->topGrossingApps(); // calling topGrossingApps

		/* PAGINATION PARAMETER */
		// You can easily add the page numbers to paginate the result
		$page = 2;
		$topGrossingApps = $class_init->topGrossingApps($page); // calling topGrossingApps

		if($topGrossingApps !== 0)
		{
			print_r($topGrossingApps); // it will show all data inside an array
		}
	</pre>
</div>

<div id="topNewPaidApps">
	<h4> Getting Top New Paid Apps </h4>
	<pre class="brush:php">
		include_once('api/playStoreApi.php'); // including class file
		$class_init = new PlayStoreApi;	// initiating class

		/* WITHOUT PARAMERTER */
		$topNewPaidApps = $class_init->topNewPaidApps(); // calling topNewPaidApps

		/* PAGINATION PARAMETER */
		// You can easily add the page numbers to paginate the result
		$page = 2;
		$topNewPaidApps = $class_init->topNewPaidApps($page); // calling topNewPaidApps

		if($topNewPaidApps !== 0)
		{
			print_r($topNewPaidApps); // it will show all data inside an array
		}
	</pre>
</div>

<div id="topNewFreeApps">
	<h4> Getting Top New Free Apps </h4>
	<pre class="brush:php">
		include_once('api/playStoreApi.php'); // including class file
		$class_init = new PlayStoreApi;	// initiating class

		/* WITHOUT PARAMERTER */
		$topNewFreeApps = $class_init->topNewFreeApps(); // calling topNewFreeApps

		/* PAGINATION PARAMETER */
		// You can easily add the page numbers to paginate the result
		$page = 2;
		$topNewFreeApps = $class_init->topNewFreeApps($page); // calling topNewFreeApps

		if($topNewFreeApps !== 0)
		{
			print_r($topNewFreeApps); // it will show all data inside an array
		}
	</pre>
</div>

<div id="topPaidGames">
	<h4> Getting Top Paid Games </h4>
	<pre class="brush:php">
		include_once('api/playStoreApi.php'); // including class file
		$class_init = new PlayStoreApi;	// initiating class

		/* WITHOUT PARAMERTER */
		$topPaidGames = $class_init->topPaidGames(); // calling topPaidGames

		/* PAGINATION PARAMETER */
		// You can easily add the page numbers to paginate the result
		$page = 2;
		$topPaidGames = $class_init->topPaidGames($page); // calling topPaidGames

		if($topPaidGames !== 0)
		{
			print_r($topPaidGames); // it will show all data inside an array
		}
	</pre>
</div>

<div id="topFreeGames">
	<h4> Getting Top Free Games </h4>
	<pre class="brush:php">
		include_once('api/playStoreApi.php'); // including class file
		$class_init = new PlayStoreApi;	// initiating class

		/* WITHOUT PARAMERTER */
		$topFreeGames = $class_init->topFreeGames(); // calling topFreeGames

		/* PAGINATION PARAMETER */
		// You can easily add the page numbers to paginate the result
		$page = 2;
		$topFreeGames = $class_init->topFreeGames($page); // calling topFreeGames

		if($topFreeGames !== 0)
		{
			print_r($topFreeGames); // it will show all data inside an array
		}
	</pre>
</div>

<div id="topTrendingApps">
	<h4>Getting Trending Apps</h4>
	<pre class="brush:php">
		include_once('api/playStoreApi.php'); // including class file
		$class_init = new PlayStoreApi;	// initiating class

		/* WITHOUT PARAMERTER */
		$topTrendingApps = $class_init->topTrendingApps(); // calling topTrendingApps

		/* PAGINATION PARAMETER */
		// You can easily add the page numbers to paginate the result
		$page = 2;
		$topTrendingApps = $class_init->topTrendingApps($page); // calling topTrendingApps

		if($topTrendingApps !== 0)
		{
			print_r($topTrendingApps); // it will show all data inside an array
		}
	</pre>
</div>

<div id="staffPicks">
	<h4> Getting Staff Picks </h4>
	<pre class="brush:php">
		include_once('api/playStoreApi.php'); // including class file
		$class_init = new PlayStoreApi;	// initiating class

		/* WITHOUT PARAMERTER */
		$staffPicks = $class_init->staffPicks(); // calling staffPicks

		/* PAGINATION PARAMETER */
		// You can easily add the page numbers to paginate the result
		$page = 2;
		$staffPicks = $class_init->staffPicks($page); // calling staffPicks

		if($staffPicks !== 0)
		{
			print_r($staffPicks); // it will show all data inside an array
		}
	</pre>
</div>

<div id="staffPicksForTablet">
	<h4> Getting Staff Picks For Tablet </h4>
	<pre class="brush:php">
		include_once('api/playStoreApi.php'); // including class file
		$class_init = new PlayStoreApi;	// initiating class

		/* WITHOUT PARAMERTER */
		$staffPicksForTablet = $class_init->staffPicksForTablet(); // calling staffPicksForTablet

		/* PAGINATION PARAMETER */
		// You can easily add the page numbers to paginate the result
		$page = 2;
		$staffPicksForTablet = $class_init->staffPicksForTablet($page); // calling staffPicksForTablet

		if($staffPicksForTablet !== 0)
		{
			print_r($staffPicksForTablet); // it will show all data inside an array
		}
	</pre>
</div>

<div id="listCategories">
	<h4> List All Categories </h4>
	<pre class="brush:php">
		include_once('api/playStoreApi.php'); // including class file
		$class_init = new PlayStoreApi;	// initiating class

		$listCategories = $class_init->listCategories(); // calling listCategories

		if($listCategories !== 0)
		{
			print_r($listCategories['Games']); // it will show all games cateogry inside an array
			print_r($listCategories['Applications']); // it will show all games cateogry inside an array
		}
	</pre>
</div>

<div id="categoryPaidItems">
	<h4>Finding Paid Items In A Category</h4>
	<pre class="brush:php">
		include_once('api/playStoreApi.php'); // including class file
		$class_init = new PlayStoreApi;	// initiating class

		/* WITHOUT PAGINATION PARAMERTER */
		$category_name = 'Themes'
		$categoryPaidItems = $class_init->categoryPaidItems($category_name); // calling categoryPaidItems

		/* PAGINATION PARAMETER */
		// You can easily add the page numbers to paginate the result
		$page = 2;
		$categoryPaidItems = $class_init->categoryPaidItems($category_name,$page); // calling categoryPaidItems

		if($categoryPaidItems !== 0)
		{
			print_r($categoryPaidItems); // it will show all data inside an array
		}
	</pre>
</div>

<div id="categoryFreeItems">
	<h4> Getting Free Items In A Category </h4>
	<pre class="brush:php">
		include_once('api/playStoreApi.php'); // including class file
		$class_init = new PlayStoreApi;	// initiating class

		/* WITHOUT PAGINATION PARAMERTER */
		$category_name = 'Themes'
		$categoryFreeItems = $class_init->categoryFreeItems($category_name); // calling categoryFreeItems

		/* PAGINATION PARAMETER */
		// You can easily add the page numbers to paginate the result
		$page = 2;
		$categoryFreeItems = $class_init->categoryFreeItems($category_name,$page); // calling categoryFreeItems

		if($categoryFreeItems !== 0)
		{
			print_r($categoryFreeItems); // it will show all data inside an array
		}
	</pre>
</div>

<div id="developerItems">
	<h4>Finding Items From A Certain Developer</h4>
	<pre class="brush:php">
		include_once('api/playStoreApi.php'); // including class file
		$class_init = new PlayStoreApi;	// initiating class

		/* WITHOUT PAGINATION PARAMERTER */
		$developer_name = 'ZYNGA'
		$developerItems = $class_init->developerItems($developer_name); // calling developerItems

		/* PAGINATION PARAMETER */
		// You can easily add the page numbers to paginate the result
		$page = 2;
		$developerItems = $class_init->developerItems($developer_name,$page); // calling developerItems

		if($developerItems !== 0)
		{
			print_r($developerItems); // it will show all data inside an array
		}
	</pre>
</div>

<div id="searchStore">
	<h4> Search Items </h4>
	<pre class="brush:php">
		include_once('api/playStoreApi.php'); // including class file
		$class_init = new PlayStoreApi;	// initiating class

		/* SEARCH PARAMETERE */
		$search_query = 'Go Themes';
		$sort = 'Popularity'	// Popularity OR Relevance ( OPTIONAL )
		$price = 'All'	// Free OR Paid OR All ( OPTIONAL )
		$safe_search = 'Off' 	// Off OR On	( OPTIONAL )

		/* WITHOUT PAGINATION PARAMERTER */
		
		$searchStore = $class_init->searchStore($search_query,$sort,$price,$safe_search); // calling searchStore

		/* PAGINATION PARAMETER */
		// You can easily add the page numbers to paginate the result
		$page = 2;
		$searchStore = $class_init->searchStore($search_query,$sort,$price,$safe_search,$page); // calling searchStore

		if($searchStore !== 0)
		{
			print_r($searchStore); // it will show all data inside an array
		}
	</pre>
</div>

<div id="itemInfo">
	<h4> Getting Item Info </h4>
	<pre class="brush:php">
		include_once('api/playStoreApi.php'); // including class file
		$class_init = new PlayStoreApi;	// initiating class

		/* WITHOUT PAGINATION PARAMERTER */
		$item_id = 'com.golauncher.go'
		$itemInfo = $class_init->itemInfo($item_id); // calling itemInfo

		if($itemInfo !== 0)
		{
			print_r($itemInfo); // it will show all data inside an array
		}
	</pre>
</div>

<div id="relatedViewed">
	<h4> Finding Related Viewed Items</h4>
	<pre class="brush:php">
		include_once('api/playStoreApi.php'); // including class file
		$class_init = new PlayStoreApi;	// initiating class

		/* WITHOUT PAGINATION PARAMERTER */
		$item_id = 'com.golauncher.go'
		$relatedViewed = $class_init->relatedViewed($item_id); // calling relatedViewed

		if($relatedViewed !== 0)
		{
			print_r($relatedViewed); // it will show all data inside an array
		}
	</pre>
</div>

<div id="relatedInstalled">
	<h4> Finding Related Installed </h4>
	<pre class="brush:php">
		include_once('api/playStoreApi.php'); // including class file
		$class_init = new PlayStoreApi;	// initiating class

		/* WITHOUT PAGINATION PARAMERTER */
		$item_id = 'com.golauncher.go'
		$relatedInstalled = $class_init->relatedInstalled($item_id); // calling relatedInstalled

		if($relatedInstalled !== 0)
		{
			print_r($relatedInstalled); // it will show all data inside an array
		}
	</pre>
</div>
