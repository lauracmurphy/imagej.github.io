---
autogenerated: true
title: Landmark Correspondences
breadcrumb: Landmark Correspondences
layout: page
author: test author
categories: Plugins,Transform,Registration
description: test description
---


{% capture author%}
{% include person content='Saalfeld' %} ([1](mailto:saalfeld@mpi-cbg.de))
{% endcapture %}

{% capture maintainer%}
{% include person content='Saalfeld' %}
{% endcapture %}

{% capture source%}
{% include github org='axtimwalde ' repo='mpicbg ' path='mpicbg\_/src/main/java/Transform\_Roi.java ' %}
{% endcapture %}
{% include info-box name='(Transform by) Landmark Correspondences ' software='Fiji ' author=author maintainer=maintainer source=source released='August 7<sup>th</sup>, 2008 ' latest-version='October 19<sup>th</sup>, 2010 ' status='stable, active ' category='[Plugins](:Category:Plugins "wikilink"), [Transform](:Category:Transform "wikilink"),[Registration](:Category:Registration "wikilink") ' %} The plugin **Landmark Correspondences** calculates a transformation between two corresponding landmark clouds and renders a transformed image. The landmarks are read from point selections over two images. The transformation is estimated by a least squares or Moving Least Squares fit for the available models.

The non-linear non-invertible transformations as estimated using the Moving Least Squares method are rendered through a mesh of triangles whose resolution is a parameter of the plugin, see [Interactive Moving Least Squares](Interactive_Moving_Least_Squares "wikilink") for an intuitive explanation.


{% capture title%}
 Two snapshots from the ImageJ Conference 2008 registered into each other using an affine transformation as estimated from automatically extracted Feature Correspondences. 
{% endcapture %}
{% include thumbnail src='/images/pages/Transform Roi-linear.jpg' title=title %} 
{% capture title%}
 A photograph and a cartoon registered into each other using the Moving Least Squares method and a similarity transformation as estimated from manually set landmark correspondences. 
{% endcapture %}
{% include thumbnail src='/images/pages/Transform Roi-mls.jpg' title=title %}

[Category:Plugins](Category:Plugins "wikilink") [Category:Transform](Category:Transform "wikilink") [Category:Registration](Category:Registration "wikilink")