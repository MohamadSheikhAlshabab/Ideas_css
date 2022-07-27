# truncate text in multiple lines(with ellipsis):

<pre>
.max-three-lines {
  -webkit-box-orient: vertical;
  display: -webkit-box;
  -webkit-line-clamp: 3;
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: normal;
}
</pre>

## Example:

#### 1.short text(1 line):

![image](https://user-images.githubusercontent.com/60566868/181302078-a45acb96-b2d8-49f7-8c3e-535a89636604.png)

#### 2.short text (2 lines):

![image](https://user-images.githubusercontent.com/60566868/181302887-cd360a65-8ff2-4dc5-8f6d-1946393a72f2.png)


#### 3. 3 lines(no overflow):

![image](https://user-images.githubusercontent.com/60566868/181302949-a38bf9eb-d196-493e-b167-1b321a886fdc.png)

#### 4.more than 3 lines:
![image](https://user-images.githubusercontent.com/60566868/181302667-fcf4ff20-9139-4896-a44a-6c92df9e6624.png)


