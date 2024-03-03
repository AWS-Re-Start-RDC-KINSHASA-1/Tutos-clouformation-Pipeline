# Tutos-clouformation-Pipeline
Plusieurs questions se posent sur la manière de créer un pipeline avec CloudFormation. Si vous vous posez la même question, alors ce tutoriel est fait pour vous ! Dans ce tutoriel, nous allons apprendre comment déployer notre infrastructure EC2 avec un pipeline. Nous allons utiliser le même code pour cet exercice. Allons-y !
Pour commencer, il faut créer un rôle pour CloudFormation en ajoutant l'accès à AmazonEC2FullAccess. Pour créer le rôle, il faut utiliser le service IAM pour cela.
![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/895cf57d-d14f-4c0a-be16-1eab42f4041d)




![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/b9f3bef7-7f85-4fa8-a39a-b2a6b7827787)





![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/82c9aaa3-48f2-4a9c-9081-3bfe09275f2a)



Choisissez CloudFormation comme option;
Ensuite, cliquez sur Suivant;



![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/fbc7533c-e89d-43f5-87b3-3bcc11f000bd)





![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/7a806e7f-15ec-4fe5-9802-60ce8a280df8)




Cliquez sur "suivant".
Ensuite, nommez votre rôle.




![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/c1bd9772-2522-4a8f-ad56-a9ff4d1175c3)





Cliquez sur "Créer un rôle";
Ensuite, allez dans CodeCommit. CodeCommit nous permettra d'exécuter notre code à partir du pipeline. Nos textes se feront dans CodeCommit.




![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/7a0db6a8-f797-49bd-8222-21dce608446c)






![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/3849de3a-66d7-4958-907f-5b2133f3658a)




Il faut créer un référentiel;




![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/2d3b9522-3cbb-42c1-9dbd-b478c508de3c)






![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/6cd810ae-4a8a-4e61-be2b-3569901a4333)





Dans l'option "Ajouter un fichier", vous allez cliquer sur "Charger un fichier". Comme je l'ai mentionné au départ, nous allons utiliser le même fichier (instance.yml).






![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/bdee6537-c747-4e2e-bca9-75b3f4e97a5b)






Maintenant, allons sur le pipeline pour déployer notre infrastructure avec CloudFormation en tant que code source provenant du code commit. Avant cela, assurez-vous d'avoir déjà créé une pile dans votre CloudFormation pour votre infrastructure EC2, car nous en aurons besoin dans le pipeline de code. Si vous ne l'avez pas encore fait, pas de problème, allez sur ce lien https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-cloud-formation-ec2-instance.git où vous trouverez les étapes pour la création.



![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/7ff0a473-8252-408f-9eeb-1e0419dbcfab)




![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/b705a387-c899-48e9-9303-c8b01d4176cb)




Nommez ensuite votre code pipeline et laissez les autres options par défaut, puis cliquez sur suivant;




![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/0b3cf519-745f-47cc-9377-f9bc103e28e0)






Dans l'option Fournisseur de code source, sélectionnez CodeCommit, puis vous verrez le référentiel et la branche. Ensuite, cliquez sur Suivant.





![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/a8f2fe3a-bbf5-4310-9e1a-f6ff0a5a21f8)


Prochaine étape cliquez sur ignorer l'étape ;


![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/6b35856d-b54a-4fd8-a367-f1e0b77f31f3)


![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/19d5c2d4-0127-4021-902b-713cb7ce2927)


Pour le fournisseur de déploiement choisissez cloud formation;



![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/4b0c4411-6cfa-4348-95f7-b3f0b655689b)


Pour le nom du fichier il faut aller voir dans code commit;



![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/c9bb2387-dc77-42e9-ba9d-98e10982ceea)

Avant de cliquer sur suivant , choisir les capacités et le rôle que vous avez créé sur IAM ;



![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/630855d0-ac04-4ae5-acc9-7022218ff082)


Ensuite cliquez suir créer;


![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/9542e21e-fed9-4bd4-8fc1-e562eae641a3)

Après avoir cliqué sur "créer", votre pipeline sera créé et un message s'affichera au-dessus indiquant que le pipeline a été effectivement créé. À côté, il y aura des cases à cocher en cours et si tout s'est bien passé, ces deux cases seront vertes, ce qui prouve que votre pipeline a fonctionné. Voici un aperçu :



![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/95002176-9115-42b6-901e-8e8f9055a834)


Passons maintenant au test. Rentrons dans notre commit pour modifier notre fichier et voir si le pipeline recevra nos modifications.
J'ai apporté des modifications sur la taille, au lieu de t2.micro c'est t2.small, et j'ai remplacé "world" par "guys".


![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/43eb2bba-ef95-4d4c-864a-6cb575600cd6)


![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/f6c48492-d815-4a6c-a8c7-9fd799bc046d)


Ensuite, retournez sur le pipeline pour vérifier si nos modifications ont été mises à jour. Il faut actualiser pour voir le processus. Cela peut prendre du temps;

![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/9bccc213-e0ac-411d-a244-ecf544310afa)

Voici le résultat final si vous avez effectué deux vérifications et que des modifications ont été apportées au pipeline;

![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/fec957b3-b629-42af-b570-e2b96c2adb90)


































