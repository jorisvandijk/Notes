# Mirroring a Git Repository

1. On Git**Hub** create a new repository, to which the repository on Git**Lab** will mirror.

2. Copy the SSH link you'd use to clone the repository. This should be *git@github.com:USERNAME/REPOSITORY.git*

3. From within a Git**Lab** project use the gear icon to select *Repository* and there go to *Mirroring repositories* and click *Expand*. 

4. In the *Git repository URL* field, paste the SSH link copied in step 2.

5. Add *ssh://* in front of the link and **replace the *:* with a */***.

6. At *Mirror direction* select *Push* (We're pushing from Git**Lab** to Git**Hub**).

7. Click the *Detect host keys* button.

8. Set *Authentication method* to *SSH Public key*.

9. Click the green *Mirror Repository* button.

10. Click the *Copy SSH public key* button, which looks like a clipboard.

11. Go back to Git**Hub**.

12. Go to *Settings* and there click on *Deploy Keys*.

13. Click the *Add deploy key* button on the top right of the page.

14. In the *Title* field add a title to identify the key. Something like *GitLab*.

15. In the *Key* field, paste the key you copied in step 10. Don't edit anything you just pasted.

16. Tick the *Allow write access* checkbox and click the *Add key* button.

17. Go back to Git**Lab**.

18. Click the *Update now* button, whick looks like two arrows.

19. Give it some time, then refresh the page and check if the *Last successful update* field changes from *Never* to *x minutes ago*.

20. You can double check by going back to Git***Hub** and refreshing the *Deploy keys* page too. *Never used* should change to *Last used within the last week — Read/write*.

21. Profit!