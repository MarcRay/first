Bienvenue a Ruby on Rails

C'est l'Apllication tir�e du livre < D�buter avec Ruby on Rails >
de Steven Holzner de Wiley Publishing Inc.
Traduction :  �dition First
ISBN : 978-2-75400-409-1

=

app
	Contient tout le code source sp�cifique � cette application.

app/assets
  Contains subdirectories for images, stylesheets, and JavaScript files.

app/controllers
	Contient le code source des contr�leurs qui doivent porter des noms du style 
	weblog_controller.rb et permettent desr�f�rences crois�es d'URL automatis�es.
	Tous les contr�leurs doivent �tre des classes descendantes de 
	ActionController::Base.
=>	Nous utiliserons syst�matiquement au moins un fichier .rb dans ce 
		sous-r�pertoire.

app/models
	Contient les mod�les qui doivent �tre li�s, dans le style post.rb.  La plupart
	des mod�les sont des descendants de ActiveRecord::Base.
=>	Nous utiliserons parfois un fichier .rb dans ce sous-r�pertoire.

app/views
	Contient les fichiers mod�les de vues dans le style weblog/index.html, dans le
	cas de l'action WeblogController#index. Les vues utilisent la syntaxe eRuby. 
	Le r�pertoire appelle �galement les feuilles de style, les images et autres 
	�l�ments qui peuvent �tre reli�s par lien symbolique vers la partie publique.
=>	Nous utiliserons presque toujours au moins un fichier .html dans ce 
		sous-r�pertoire. 

app/views/layouts
  Holds the template files for layouts to be used with views. This models the
  common header/footer method of wrapping views. In your views, define a layout
  using the <tt>layout :default</tt> and create a file named default.html.erb.
  Inside default.html.erb, call <% yield %> to render the view using this
  layout.

app/helpers
Contient les assistants de vues avec des noms dans le style weblog_helper.rb.


app/apis
	Contient les classes de l'interface API pour les services Web.

config
	Contient les fichiers de configuration de l'environnement Rails, la carte de 
	routage, la base de donn�es et les autres d�pendances.
=>	Nous utiliserons parfois un fichier  .rb dans ce sous-r�pertoire.

components
	Contient des mini-apllications autonomes qui peuvent �tre reli�es ensemble via 
	des contr�leurs, des mod�les et des vues.
	
db
	Contient le sch�ma de base de donn�es dans le fichier schema.rb. Le 
	sous-r�pertoire db/migrate contient la totalit� de la s�quence des migrations
	de votre base de donn�es.

doc
  This directory is where your application documentation will be stored when
  generated using <tt>rake doc:app</tt>

lib
	Contient les librairies sp�cifiques de l'application (bibliot�que). Re�oit dans
	la pratique tout le code sp�cifique qui peut �tre plac� avec les contr�leurs,
	les mod�les ou les assistants. Ce r�pertoire est mentionn� dans le chemin de
	chargement load path.

public
	C'est le r�pertoire accessible aux serveurs Web. Il contient des sous-r�pertoires
	pour les images, les distributeurs et les fichiers HTML par d�faut.
=>	Nous y cr�erons parfois un ou deux fichier  .html.

script
  Contient les scripts d'assistances � l'automatisation et � la g�n�ration.

test
	Contient les tests unitaires et fonctionnels ainsi que les accessoires (fixtures).

vendor
	Contient les librairies externes dont l'application � besion ainsi que le 
	sous-r�pertoire des extensions plugins.
	
  
