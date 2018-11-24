# weka-smote-clustering
can you please help me ,i want to cluster the subdataset  (sample)
i want to add something like,

/*
{

  SimpleKMeans kmeans = new SimpleKMeans();
 
  kmeans.setNumClusters(2);

  kmeans.buildClusterer(sample);

  weka.core.Instances[] datasets = new weka.core.Instances[kmeans.getNumClusters()]; 

   for (int i = 0; i < datasets.length; i++) 

   {
 
   datasets[i] = new Instances(sample, 0);
 
   }

   for (Instance inst : sample)

   {
 
   datasets[(int)kmeans.clusterInstance(inst)].add(inst);

   }

  }

*/

but it does not seems to work,   after compiling the weka program using ANT EXEJAR command, with modifying SMOTE.java . The new weka app is created with the modified filter SMOTE.java,  but when i run the program and use the filter it gives me the following error :

 weka java problem filtering instances: weka.clusterers.SimpleKMeans: Cannot handle any class attribute! 

could you please help me with this matter
