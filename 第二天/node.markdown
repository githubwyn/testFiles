## ���������ص�

    1.��������������һ��$scope,
    2.����ע��
    3.DOM����������÷�Χƽ��
    4.����������Ƕ��ʹ�ã�ע��Ƕ�׵���DOM��ǩ
    5.���������ܸ��ã��������ý����ǿ���Ψһ���Բ����ĵط�
    
    
##  ng-options="option.id as option.title for option in curOptionArray"

    ��������һ��ng���﷨ 
    option.id��select�ύ��ֵ 
    option.title��select��ʾ��ֵ 
    option��������curOptionArray����ĵ�ǰԪ��
    
    $sce �����ǰ�htmlת���
    ����ע�룺��ֻҪ��ʹ�ã���Ҫ������ע�����
    
## ָ��---��չ���ܣ���װ���

    װ����ָ����������ӹ��ܣ�
    �����ָ�� ������һЩ���ܣ�ʵ�����絯�㣬����Ч����
    
    ָ�������ȫ������������
    ͨ��ģ��������ָ��
    ������ǩ�Ĺ淶����ǩ�ﲻ���ִ�д��ĸ
    myHello----->��һ������������ָ������
    template:'<h>hello</h><p>jlsajlkj</p>' -----> �ڶ���������������Ĭ�Ϸ��ض���
    
    var app=angular.module('appModule',[]);
        app.directive('myHello',function(){
            return {
                template:`<h>hello</h><p>jlsajlkj</p>`
            }
        })
        
        
    var app=angular.module('appModule',[]);
        app.directive('drag',function(){
            return {
                //link����ʱΨһһ�����Բ���dom�ĵط�,�����ǵ���ͼ�����ݽ��а󶨵ģ����Ӻ�����
                link:function(scope,element,attrs){
                    //angular.element(div);//angular.element��ס�Ķ������һ��jQuery����
                    //scope����ǰԪ��
                    //element��ǰָ�����ڵ�Ԫ��Ĭ��Ϊjq����
                    // attrs��ʾ��ǰԪ������
                }
            }
        })
        
##  ����es6�ı�ǩʵ���ַ�������ƴ��-----ǰ���������µ�wb�汾
    
    �÷�������
    var name='zf';
    var age=8;
    console.log(``)

    ``
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    

