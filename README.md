# Classification automatique à partir de texte et d'image

Ce projet est basé sur les données disponibles à [cette adresse](https://s3-eu-west-1.amazonaws.com/static.oc-static.com/prod/courses/files/Parcours_data_scientist/Projet+-+Textimage+DAS+V2/Dataset+projet+pre%CC%81traitement+textes+images.zip).  
Il consiste à chercher à classer automatiquement les objets d'un site de e-commerce à partir de la photo et du texte descriptif. J'ai fait le choix de travailler séparément sur le texte et les photos, les résultats n'étant pas très probants, je n'ai pas cherché à combiner les deux.  

Dans le premier notebook, les données sont mises en forme et les objets mis en clusters en utilisant uniquement le texte (bag of words et word embedding). Les clusters obtenus sont comparés à la classification existante.  
Dans le deuxième notebook, les objets sont mis en clusters à partir des images (descripteurs ORB et bag of visual words).  
Dans le troisième, un classifieur BERT est adapté par transfer learning pour une classification supervisée à partir du texte.  
Dans le quatrième, un classifieur VGG16 est adapté par transfer learning pour une classification supervisée à partir des images.

