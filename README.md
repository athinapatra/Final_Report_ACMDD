# ACMDD_REPORT
**Andrianopoulou Vasiliki (s3222160)
Byrne Vania (s3254062)
Patra Athina (s3364348)
Protein of interest: JNK-1
PDB ID: 2GMX** 



**1. INTRODUCTION**

c-Jun N-terminal kinase-1 (JNK-1) is a member of the superfamily of MAP kinases (Mitogen Activated Protein kinases) and is alternatively described with the name MAPK8 (PDB ID 2GMX). The MAPK8 gene is located in the 10q11.22 chromosomal locus and encodes for a 427 amino acids protein of a molecular weight of 48 kDa. MAP kinases bind and phosphorylate other proteins in Serine/Threonine (Ser/Thr) residues in order to activate them and are involved in a plethora of cellular processes including cell proliferation, differentiation, transcription regulation, development, and apoptosis. Additionally, JNK kinases are highly conserved among species and consist of 10 isoforms resulting from several alternative splicing events in three genes; four isoforms derived from JNK-1, four isoforms derived from JNK-2, and three isoforms derived from JNK-3. Moreover, JNK-1 and JNK-2 often have redundant functions and are ubiquitously expressed in most human tissues, whilst JNK-3 is mainly expressed in the brain and testes. JNK proteins consist of a small N-terminal domain with β-strands and a large C-terminal domain with α-helices. The N-terminal domain connects with the C-terminal domain through a flexible hinge-like region, where a cleft with the ATP-binding site can be found.
JNK1 is activated by dual phosphorylation of Threonine (Thr) and Tyrosine (Tyr) residues in the Thr-Pro-Tyr motif located in the kinase subdomain VIII of the protein by MAP2K4/MKKK4 and MAP2K7/MKKK7, and acquires its inactive form after dephosphorylation by Ser/Thr and Tyr phosphatases. MAP kinases are activated due to cellular stress stimuli, such as pro-inflammatory cytokines, changes in the ROS (reactive oxygen species) levels, heat shock, UV irradiation, hypoxia, and chemotoxins. Upregulation of JNK-1 has been associated with several types of cancer development and progression, such as human pancreatic, lung, breast, skin cancer, B-lymphoma, and osteosarcoma, thus JNK-1 is considered a proto-oncogene. JNK-1 regulates the activity of various proteins such as c-Jun, ATF-2, p53, c-Myc, and STAT3, which are either located in the cytoplasm or migrate to the nucleus to activate transcription factors. Activation of the JNK pathway is associated with the coordination of scaffold proteins of the JNK activation complex that amplify the biochemical signal. 
Much collaborative effort has been made to produce small molecule JNK-1 inhibitors to circumvent tumorigenesis associated with JKN signalling. A plethora of such inhibitors has been developed that are ATP-competitive or ATP-non-competitive with reversible binding, selective or non-selective of specific JNK isoforms, some of which have already reached clinical trials. In this project, we particularly focused on two JNK-1 inhibitors, namely Tanzisertib (CC-930) and CC-401 that reached clinical trial phases IIa and I, before being retrieved from further research. These compounds were used by our group as models to generate our own molecules for docking studies. More specifically, Tanzisertib (CC-930) is a first-generation potent, ATP-competitive inhibitor, selective for JNK proteins. It was used for the treatment of idiopathic pulmonary fibrosis and discoid lupus erythematosus, but due to efficacy issues, it was discontinued in 2012. Lastly, CC-401 is a second-generation potent ATP-competitive JNK inhibitor. It has been used for renal injury studies and was discontinued after clinical phase I, for acute myeloid leukemia. Nonetheless, both of these compounds could be used as starting points in our project and show promising potential as tools in docking. Perhaps small alterations of these molecules could result in the development of better selective JNK inhibitors in the future with high efficiency and low adverse effects.
In the code file the python code that was used in the search for novel JNK-1 inhibitors can be found.

**2. DISCUSSION**

During the similarity investigation, we searched three different databases which comprise large repositories of millions of freely accessible compounds. Particularly, in ChEMBL no similar compounds were obtained when setting the similarity index to 80%, whereas in the PubChem database we obtained 6 compounds with 90% similarity and 125 compounds when the similarity index was set to 80%. This can be explained by the fact that in PubChem 329 million compounds are registered whereas in ChEMBL only 2.5 million compounds can be found. Finally, the Zinc database contains over 230 million purchasable compounds, in ready-to-dock 3D formats, in which 4 compounds were obtained with a similarity of 70% to our ligand. For the Machine Learning part of the study, we downloaded compounds from ChEMBL.
In the Machine Learning as well as in the docking exercises we tried to run different molecules based on the two chemical structures of the compounds that have reached the clinical phase I and I, targeting JNK1. Taking into account our reference co-crystallized ligand we got a deeper insight into its main interactions with our protein of interest, JNK1, using the Protein Ligand Interaction Profiler (PLIP). In this way, we could generate derivatives that entail similar interactions with amino acids existing in close proximity to the binding site. 

<img width="553" alt="Screenshot 1" src="https://user-images.githubusercontent.com/118119791/201532471-12de388f-f3eb-4074-aa33-8a808b8da033.png">

Looking into the first illustration of the ligand inside the binding pocket we observe that the main interactions are obtained through two hydrogen bonds; one between the NH2 group of the ligand and the oxygen of a glutamine close to the binding site and another one between the carbonyl group of the ligand and the amine of methionine existing in close proximity to the binding site. In addition, hydrophobic interactions are observed between the aromatic ring and the amino acid of isoleucine as well as between the ligand and methionine.

<img width="343" alt="Screenshot 2" src="https://user-images.githubusercontent.com/118119791/201531624-55feb648-cec9-4630-a18e-3b92d0d69891.png">

In the second illustration, we can observe additional interactions between the ligand and JNK1. More specifically, we observe one additional hydrogen bond between the nitrogen of the cyano moiety and a lysine as well as one between the oxygen which is in meta position to the bromine and asparagine. Moreover, four more hydrophobic interactions are observed. These interactions are mainly the results of interactions between the aromatic rings and adjacent amino acids. Lastly, the halogen bond between the bromine and a lysine seems to stabilize even more the ligand inside the binding pocket.

Taking into account these interactions as well as the structures of the two most promising compounds that underwent phase II of clinical trials we move on to the generation of new molecules. First, having noticed a variety of hydrogen bonds forming between nitrogen atoms and proximal amino acids, we substituted the fluorine atoms with an amino group. However, we observed a slightly  lower pIC50 of 7.05 compared to the parent compound which presented a pIC50 of 7.17, indicating that the fluorine atoms are actually essential for more efficient binding to our protein of interest. The reason behind that could be that the electron-withdrawing properties of the fluorine atoms make the nitrogen more electrophilic, thus forming stronger hydrogen bonds with the close-by amino acids. In addition, the halogen bonds of the fluorine atoms might significantly stabilize the ligand inside the binding pocket.

<img width="598" alt="Screenshot 3" src="https://user-images.githubusercontent.com/118119791/201531792-cf4a7dc0-1929-4331-95cc-d507fba17a00.png">

Following we can see some docking poses of the generated molecule which presented a docking score of -8.100 kcal/mol compared to the parent compound for which we obtained a docking score of -7.840 kcal/mol.

<img width="511" alt="Screenshot 4" src="https://user-images.githubusercontent.com/118119791/201531806-da4c50b6-0ab2-4255-99a3-0f3f009213f5.png">

Next, we explored the influence of an additional amino group in the meta position on the existing amino group. A further decrease of the pIC50 (6.91) indicated that no significant interactions were obtained with this modification. In contrast, this modification might cause steric hindrance, not allowing in this way, the formation of possible hydrogen bonds of the adjacent amine with the respective amino acids.

<img width="624" alt="Screenshot 5" src="https://user-images.githubusercontent.com/118119791/201531831-2c13b383-f44c-4d9d-a177-bc65c6d91f6a.png">

The docking score obtained for this molecule was -8.002 kcal/mol. Generally, we noticed a contradictory relationship between the docking scores and the pIC50 values, indicating that we should further investigate and take into account the reasons behind this. 

<img width="607" alt="Screenshot 6" src="https://user-images.githubusercontent.com/118119791/201531845-1e6052d5-9420-418f-a59c-22762381fd38.png">

For our second parent compound, we generated one more molecule. Following a similar strategy, we substituted the piperidine ethyl ether group with an amino group. The pIC50 of 6.07 was slightly lower than the one of the parent compound which presented a pIC50 of 6.09. Therefore, a hydrogen bond from the ether’s oxygen in combination with hydrophobic interactions generated by the ethyl chain might stabilize this configuration compared to the generated molecule. However, the ability of the nitrogen to form stable hydrogen bonds might be the reason why the pIC50 is still comparable to the one of the parent compound.

<img width="607" alt="Screenshot 7" src="https://user-images.githubusercontent.com/118119791/201531866-0dd7bdda-5425-4cb3-ab25-9b22a8e8b342.png">

Following we can see some docking poses of the generated molecule which presented a docking score of -8.537 kcal/mol compared to the parent compound which presented a docking score of -8.786 kcal/mol.

<img width="1440" alt="Screenshot 8" src="https://user-images.githubusercontent.com/118119791/201531874-a640eb6e-b68b-4cf4-9505-fe2bfc7a7763.png">

**3. References**

1. U.S. National Library of Medicine. (n.d.). MAPK8 mitogen-activated protein kinase 8 [homo sapiens (human)] - gene - NCBI. National Center for Biotechnology Information. Retrieved November 13, 2022, from https://www.ncbi.nlm.nih.gov/gene/5599 
2. Wu Q, Wu W, Jacevic V, Franca TCC, Wang X, Kuca K. Selective inhibitors for JNK signalling: a potential targeted therapy in cancer. J Enzyme Inhib Med Chem. 2020;35(1):574-583. doi:10.1080/14756366.2020.1720013
3. Yi P, Qiu M. 3D-QSAR and docking studies of aminopyridine carboxamide inhibitors of c-Jun N-terminal kinase-1. Eur J Med Chem. 2008;43(3):604-613. doi:10.1016/j.ejmech.2007.04.020
4. Duong MTH, Lee JH, Ahn HC. C-Jun N-terminal kinase inhibitors: Structural insight into kinase-inhibitor complexes. Comput Struct Biotechnol J. 2020;18:1440-1457. doi:10.1016/j.csbj.2020.06.013
5. Szczepankiewicz BG, Kosogof C, Nelson LTJ, et al. Aminopyridine-based c-Jun N-terminal kinase inhibitors with cellular activity and minimal cross-kinase activity. J Med Chem. 2006;49(12):3563-3580. doi:10.1021/jm060199b
6. Sydow D, Morger A, Driller M, Volkamer A. TeachopenCadd: A teaching platform for computer-aided drug design using open source packages and data. J Cheminform. 2019;11(1):1-7. doi:10.1186/s13321-019-0351-x
