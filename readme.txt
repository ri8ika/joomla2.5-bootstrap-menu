1. First place the following html inside your template index.php file:

<nav class="navbar navbar-default navbar-fixed-top">
  <div class="container-fluid">
    <!-- Brand and toggle get grouped for better mobile display -->
    <div class="navbar-header">
      <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#main-navigation" aria-expanded="false">
        <span class="sr-only">Toggle navigation</span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
      </button>
      <a class="navbar-brand" href="<?php echo $this->baseurl;?>" id="logo"><img src="<?php echo $this->baseurl ?>/<?php echo htmlspecialchars($logo); ?>" alt="<?php echo htmlspecialchars($templateparams->get('sitetitle'));?>" /></a>
    </div>

    <!-- Collect the nav links, forms, and other content for toggling -->
    <div class="collapse navbar-collapse" id="main-navigation">
    	<jdoc:include type="modules" name="mainnavigation" style="none" />
    </div><!-- /.navbar-collapse -->
  </div><!-- /.container-fluid -->
</nav>

2. Then in your templates/html/mod_menu put the following files:

default.php
default_url.php
default_component.php

3. In your css file, put the following code:

.dropdown:hover > ul {
    display: block;
}

Best Regards,
Bhojendra Rauniyar