###Todo
  avant de te casser la tete essaie de comprendre le code source et vois les css qui y sont appliqué 
 
 regle le pb de editor ce week-end 
https://www.drupal.org/forum/support/post-installation/2018-02-07/i-dont-have-an-html-no-editor-option-for-text-format-for  

## A noter ds iblb  ++++++
[] pour editer un text sans formattage dans les bloc.
  il faut : aller dans config  et creer un type de redaction :  http://localhost/ibdrupal/web/admin/config/content/formats
    → add text format    cree un type de format pour le plain text et SELECTIONNE NO EDITOR 
	  comme ckeditor ny est pas et le formatage  html ne sera pas appliqué , il sera brut et tu appliquerer ton csss comm tu veux 

## quand tu cree une modif , toujours verifier 
   exemple quand tu cree les regions ds infos , verifie que cest pri en compte en faisant lanancant la demo ds structure : 
     exemple http://localhost/ibdrupal/web/admin/structure/block/demo/octo



[for drupal pour avo]
A GERER 
   REPRENDRE LE THEE DEPUIS LE DEBUT 
    ET SUIVRE AVEC DRUPAL LES RECOMMENDATION  et note dans IBLB 
	
► https://www.drupal.org/docs/develop/theming-drupal
   ► https://www.drupal.org/docs/develop/theming-drupal/adding-regions-to-a-theme
       tres important note bien la gestion des regions si tu veux recuperer les regions copie les et ajoutes tiennes 
       car toute fois que tu met le keyword regions dans info.yml tu ecrase la source donc si tu le veux ecopoie l 'existant et je pense que 
        si ca n'esxiste pas , il herite la preuse quand tu cree le theme avec cmline , il cree sans region 

      maintenant toute regions declaré dans info doit etre notée dans un template twig 		
	 
  ► https://www.drupal.org/docs/develop/theming-drupal/adding-assets-css-js-to-a-drupal-theme-via-librariesyml    [TODO+++ IN PROGRESS]
          Le tuto in progress  1. comprendre comment les ccs jont ajoué  (voir ce lien)
		                       2. comment verifier que mes css sont cahrgé et js 
							   3. lire son css et test apply 
							   4. que dis le html que tu veux modifier 
							   5. demande a chat gpt 
	   
    
  
  ► adding assets-css-js to drupal
 https://www.drupal.org/node/2274843
     
https://salsa.digital/insights/mastering-drupal-theming-basics-brilliance






### another tmp to master  css 
  the chalenge and the test is to 
  create something in a block and apply a registered css to it 
    
  https://www.youtube.com/watch?v=BX-HxH3MhAw

https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Styling_basics/Debugging_CSS

https://www.youtube.com/watch?v=ndeClnyHSo8


https://medium.com/@wolfflucas/how-to-debug-css-with-css-fd66de34ba59

https://joyofcode.xyz/simple-css-debug-trick

https://whitep4nth3r.com/blog/debug-css-layouts/

https://debuggingcss.com/
vhttps://www.smashingmagazine.com/2021/10/guide-debugging-css/

https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Styling_basics/Debugging_CSS



  ### A gerer  del si ncessaire 	

composer require 'drupal/backup_migrate:^5.0'


consoles 	

document.styleSheets

Dans l'outil d'inspection, sélectionne un élément de la page et va dans l'onglet "Styles".

Cherche les règles de style de ton fichier CSS appliquées à cet élément.

