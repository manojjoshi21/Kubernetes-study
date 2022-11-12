1.Create a new pod with the nginx image
    k run nginx --image=nginx

2. k create deployment httpd-frontend --replicas=3 --image=httpd:2.4-alpine

3. Update image 
 k create deployment nginx-deployment --replicas=3 --image=nginx:1.14.2
 kubectl set image deployment/nginx-deployment nginx=nginx:1.16.1
 kubectl rollout status deployment/nginx-deployment
 kubectl rollout history deployment/nginx-deployment
 kubectl rollout history deployment/nginx-deployment --revision=1
 kubectl rollout history deployment/nginx-deployment --revision=2

 4. Undo deployment

 k rollout undo deployment/nginx-deployment

 Alternatively, you can rollback to a specific revision by specifying it with --to-revision:

 kubectl rollout undo deployment/nginx-deployment --to-revision=2

5.  Scaling deployment
    kubectl scale deployment/nginx-deployment --replicas=10

6. Rollout pause
   kubectl rollout pause deployment/nginx-deployment
   Rollout resume
   kubectl rollout resume deployment/nginx-deployment

7. 