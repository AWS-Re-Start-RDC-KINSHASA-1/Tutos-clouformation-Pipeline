# Tutos-clouformation-Pipeline
Plusieurs questions sont posées de savoir comment faire du pipeline avec cloudformation, si vous vous posez la même question alors ce tuto est fait pour vous ! Dans ce tutos nous allons apprendre comment deployer notre infrastructure ec2 avec pipeline . nous allons utilisé le même code pour cet exercice . let's go! 
Pour ce faire il faut créer un rôle pour cloud formation en ajoutant l'accès à AmazonEC2FullAcess . pour créer le rôle il faut utilisé le service IAM pour ça;

![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/895cf57d-d14f-4c0a-be16-1eab42f4041d)




![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/b9f3bef7-7f85-4fa8-a39a-b2a6b7827787)





![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/82c9aaa3-48f2-4a9c-9081-3bfe09275f2a)



Choisissez Cloud formation comme option;
Ensuite cliquez sur suivant;



![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/fbc7533c-e89d-43f5-87b3-3bcc11f000bd)





![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/7a806e7f-15ec-4fe5-9802-60ce8a280df8)




Cliquez sur suivant;
Ensuite nomez votre rôle;




![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/c1bd9772-2522-4a8f-ad56-a9ff4d1175c3)





Cliquez sur créer un rôle;
Ensuite allez dans code commit, code commit nous permettra d'éxecuter notre code à partir du pipeline . Nos text se feront dans code commit;





![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/7a0db6a8-f797-49bd-8222-21dce608446c)






![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/3849de3a-66d7-4958-907f-5b2133f3658a)




Il faut créer un référentiel;




![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/2d3b9522-3cbb-42c1-9dbd-b478c508de3c)






![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/6cd810ae-4a8a-4e61-be2b-3569901a4333)





Dans l'option ajouter un fichier vous allez cliquer charger un fichier . comme je le dis au départ nous allons utilisé le même fichier(instance.yml);






![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/bdee6537-c747-4e2e-bca9-75b3f4e97a5b)






Maintenant , allons sur pipeline pour deployer notre infrastructure avec cloud formation comme code source venant du code commit , mais avant ça il faut s'assurer que vous avez déja créer une pile dans votre cloud formation pour votre infranstrure ec2 nous en aurons besoin dans code pipeline , si vous ne l'avez pas fait , pas de problème allez sur ce lien  https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-cloud-formation-ec2-instance.git vous trouverez les étapes pour créer.



![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/7ff0a473-8252-408f-9eeb-1e0419dbcfab)




![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/b705a387-c899-48e9-9303-c8b01d4176cb)




Ensuite nommez votre code pipeline et laissez les autres options par défaut ensuite cliquer sur suivant;




![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/0b3cf519-745f-47cc-9377-f9bc103e28e0)






Dans l'option fournisseur du code source , choisissez code commit ensuite  vous verrez le reférentiel et la branche ensuite cliquez sur suivant ;





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

Après avoir cliquer sur créer , votre pipeline sera créé et il y'aura un message au dessus qui indique que le pipeline a été vraiment créé et à côté y'aura de check en cours et si tout a été bient ses deux checks seront en vert ce qui prouve que votre pipeline a marché , voici un aperçu;



![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/95002176-9115-42b6-901e-8e8f9055a834)


Passons maintenat au test . rentront dans notre commit pour modifier notre fichier et voir si le pipelin réçevra nos modifications.
J'ai apporté de modification sur la taille au lieu t2.micro c'est t2.small  et j'ai remplacé le world par guys .


![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/43eb2bba-ef95-4d4c-864a-6cb575600cd6)


![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/f6c48492-d815-4a6c-a8c7-9fd799bc046d)


Ensuite rentrez sur pipeline pour voir si nos modifications ont été mises à jours , il faut actualisez pour voir le processus. ça peut prendre du temps ;

![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/9bccc213-e0ac-411d-a244-ecf544310afa)

Voici le résultat final si vous avez deux check donc les modifications ont été apportés sur pipeline;

![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/fec957b3-b629-42af-b570-e2b96c2adb90)


































