Bienvenue a Ruby on Rails

C'est l'Apllication tirée du livre < Débuter avec Ruby on Rails >
de Steven Holzner de Wiley Publishing Inc.
Traduction :  Édition First
ISBN : 978-2-75400-409-1

=

app
	Contient tout le code source spécifique à cette application.

app/assets
  Contains subdirectories for images, stylesheets, and JavaScript files.

app/controllers
	Contient le code source des contrôleurs qui doivent porter des noms du style 
	weblog_controller.rb et permettent desréférences croisées d'URL automatisées.
	Tous les contrôleurs doivent être des classes descendantes de 
	ActionController::Base.
=>	Nous utiliserons systématiquement au moins un fichier .rb dans ce 
		sous-répertoire.

app/models
	Contient les modèles qui doivent être liés, dans le style post.rb.  La plupart
	des modèles sont des descendants de ActiveRecord::Base.
=>	Nous utiliserons parfois un fichier .rb dans ce sous-répertoire.

app/views
	Contient les fichiers modèles de vues dans le style weblog/index.html, dans le
	cas de l'action WeblogController#index. Les vues utilisent la syntaxe eRuby. 
	Le répertoire appelle également les feuilles de style, les images et autres 
	éléments qui peuvent être reliés par lien symbolique vers la partie publique.
=>	Nous utiliserons presque toujours au moins un fichier .html dans ce 
		sous-répertoire. 

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
	routage, la base de données et les autres dépendances.
=>	Nous utiliserons parfois un fichier  .rb dans ce sous-répertoire.

components
	Contient des mini-apllications autonomes qui peuvent être reliées ensemble via 
	des contrôleurs, des modèles et des vues.
	
db
	Contient le schéma de base de données dans le fichier schema.rb. Le 
	sous-répertoire db/migrate contient la totalité de la séquence des migrations
	de votre base de données.

doc
  This directory is where your application documentation will be stored when
  generated using <tt>rake doc:app</tt>

lib
	Contient les librairies spécifiques de l'application (bibliotèque). Reçoit dans
	la pratique tout le code spécifique qui peut être placé avec les contrôleurs,
	les modèles ou les assistants. Ce répertoire est mentionné dans le chemin de
	chargement load path.

public
	C'est le répertoire accessible aux serveurs Web. Il contient des sous-répertoires
	pour les images, les distributeurs et les fichiers HTML par défaut.
=>	Nous y créerons parfois un ou deux fichier  .html.

script
  Contient les scripts d'assistances à l'automatisation et à la génération.

test
	Contient les tests unitaires et fonctionnels ainsi que les accessoires (fixtures).

vendor
	Contient les librairies externes dont l'application à besion ainsi que le 
	sous-répertoire des extensions plugins.
	
  
