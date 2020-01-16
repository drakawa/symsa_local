# symsa_local

This is a patch for https://github.com/mnakao/GraphGolf.git Revision 20d355a00d729a5cadcbde96629558a0c73e49d5 (Commits on Dec 3, 2019) to create symsa_local($\sigma$) topologies.

# Added Option
* -l : Minimum number of lines (links) in each group (> 0, integer)

# Example of execution
    $ mpirun -np 1 ./gg -f ./data/n16d4.random.edges -g 4 -l 16 -o n64d4g4l16.edges
    
* min_links = n * d * $\sigma$ / 2
* i.e. $\sigma$ = 2 * min_links / (n * d)
* ($\sigma$ = 2 * 16 / (16 * 4) = 0.5 in this example)
