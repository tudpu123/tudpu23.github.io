// 前端代码 - 发起支付请求
async function directPay(orderData) {
    try {
        const response = await fetch('https://2a.mazhifupay.com/api/pay', {
            method: 'POST',
            headers: {
                'Content-Type': 'application/json',
            },
            body: JSON.stringify({
                merchant_id: '131517535',
                key: '6K1yVk6M16BK72Ms2ZB8wEyM020bZxK2',
                order_no: orderData.orderNo,
                amount: orderData.amount,
                // 其他必要参数
            })
        });
        
        const result = await response.json();
        if (result.code === 200) {
            // 支付成功处理
            console.log('支付成功');
        }
    } catch (error) {
        console.error('支付失败:', error);
    }
}
