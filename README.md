# -.github.io
我的个人 HTML 静态网站
[Uploading 三端优化版 - 副本.html…]()
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=5.0, user-scalable=yes">
    <meta name="apple-mobile-web-app-capable" content="yes">
    <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
    <meta name="format-detection" content="telephone=no">
    <meta name="theme-color" content="#4A86E8">
    <title>财财cos后期价格速算</title>
    <style>
        /* ===== CSS重置和基础样式 ===== */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            -webkit-tap-highlight-color: transparent;
            -webkit-text-size-adjust: 100%;
            -moz-text-size-adjust: 100%;
            -ms-text-size-adjust: 100%;
            -webkit-font-smoothing: antialiased;
            -moz-osx-font-smoothing: grayscale;
        }

        html {
            font-size: 16px;
            height: 100%;
            -webkit-text-size-adjust: 100%;
            -moz-text-size-adjust: 100%;
            -ms-text-size-adjust: 100%;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, "PingFang SC", "Hiragino Sans GB", "Microsoft YaHei", "Helvetica Neue", Arial, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            padding: 15px;
            line-height: 1.5;
            color: #333;
            overflow-x: hidden;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        /* ===== 主容器 ===== */
        .container {
            width: 100%;
            max-width: 1000px;
            background: rgba(255, 255, 255, 0.95);
            padding: clamp(15px, 4vw, 25px);
            border-radius: clamp(12px, 2vw, 20px);
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.1);
            margin: 0 auto;
            backdrop-filter: blur(10px);
            position: relative;
            z-index: 1;
        }

        /* ===== 标题区域 ===== */
        .header {
            text-align: center;
            margin-bottom: clamp(20px, 4vw, 30px);
            padding-bottom: clamp(15px, 3vw, 20px);
            border-bottom: 2px solid #e8f4ff;
        }

        .main-title {
            font-size: clamp(1.6rem, 5vw, 2.2rem);
            color: #333;
            margin-bottom: 10px;
            font-weight: 700;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .subtitle {
            font-size: clamp(0.85rem, 3vw, 0.95rem);
            color: #666;
            line-height: 1.5;
            padding: 0 clamp(10px, 2vw, 20px);
            max-width: 800px;
            margin: 0 auto;
        }

        /* ===== 分区样式 ===== */
        .section {
            background: #f8f9fa;
            border-radius: clamp(10px, 2vw, 15px);
            padding: clamp(15px, 3vw, 20px);
            margin-bottom: clamp(15px, 3vw, 20px);
            border: 1px solid #e9ecef;
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .section:hover {
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.08);
            transform: translateY(-2px);
        }

        .section-title {
            font-size: clamp(1rem, 3.5vw, 1.2rem);
            color: #333;
            margin-bottom: clamp(15px, 3vw, 20px);
            font-weight: 600;
            padding-bottom: clamp(8px, 1.5vw, 10px);
            border-bottom: 2px solid #4A86E8;
            display: flex;
            align-items: center;
        }

        .section-title::before {
            content: '';
            display: inline-block;
            width: 4px;
            height: 20px;
            background: #4A86E8;
            margin-right: 10px;
            border-radius: 2px;
        }

        /* ===== 按钮组 ===== */
        .btn-group {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
            gap: clamp(10px, 2vw, 15px);
            margin-bottom: clamp(15px, 3vw, 20px);
        }

        .btn {
            padding: clamp(12px, 2.5vw, 15px);
            border: none;
            border-radius: 10px;
            font-size: clamp(0.9rem, 3vw, 1rem);
            font-weight: 500;
            cursor: pointer;
            text-align: center;
            transition: all 0.3s ease;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 8px;
            min-height: 44px; /* iOS点击友好尺寸 */
        }

        .btn:active {
            transform: scale(0.98);
        }

        .clear-btn {
            background: linear-gradient(135deg, #ff6b6b 0%, #ff4757 100%);
            color: white;
            box-shadow: 0 4px 12px rgba(255, 107, 107, 0.3);
        }

        .clear-btn:hover {
            background: linear-gradient(135deg, #ff5252 0%, #ff3838 100%);
            box-shadow: 0 6px 18px rgba(255, 107, 107, 0.4);
        }

        .add-btn {
            background: linear-gradient(135deg, #4A86E8 0%, #3a76d8 100%);
            color: white;
            box-shadow: 0 4px 12px rgba(74, 134, 232, 0.3);
        }

        .add-btn:hover {
            background: linear-gradient(135deg, #3a76d8 0%, #2a66c8 100%);
            box-shadow: 0 6px 18px rgba(74, 134, 232, 0.4);
        }

        /* ===== 空状态提示 ===== */
        .empty-tip {
            text-align: center;
            color: #999;
            padding: clamp(30px, 6vw, 50px) clamp(15px, 3vw, 30px);
            font-style: italic;
            font-size: clamp(0.9rem, 3vw, 1rem);
            background: rgba(255, 255, 255, 0.7);
            border-radius: 10px;
            border: 2px dashed #e0e0e0;
        }

        /* ===== 服务池 ===== */
        .service-pool {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(160px, 1fr));
            gap: clamp(10px, 2vw, 15px);
            margin-top: clamp(15px, 3vw, 20px);
        }

        .service-item {
            display: flex;
            align-items: center;
            padding: clamp(12px, 2.5vw, 15px);
            background: white;
            border: 2px solid #e0e0e0;
            border-radius: 12px;
            cursor: pointer;
            transition: all 0.3s ease;
            user-select: none;
        }

        .service-item:hover {
            border-color: #4A86E8;
            box-shadow: 0 4px 12px rgba(74, 134, 232, 0.15);
            transform: translateY(-2px);
        }

        .service-item.checked {
            border-color: #4A86E8;
            background: rgba(74, 134, 232, 0.05);
            box-shadow: 0 4px 12px rgba(74, 134, 232, 0.2);
        }

        .service-checkbox {
            margin-right: clamp(8px, 1.5vw, 12px);
            width: 20px;
            height: 20px;
            cursor: pointer;
            accent-color: #4A86E8;
            flex-shrink: 0;
        }

        .service-name {
            font-weight: 500;
            color: #333;
            font-size: clamp(0.9rem, 2.5vw, 1rem);
            flex: 1;
            word-break: break-word;
        }

        /* ===== 已选服务项 ===== */
        .selected-services-list {
            min-height: 60px;
        }

        .selected-item {
            background: white;
            padding: clamp(15px, 3vw, 20px);
            border: 1px solid #e0e0e0;
            border-radius: 12px;
            margin-bottom: clamp(12px, 2vw, 15px);
            position: relative;
            overflow: hidden;
            transition: all 0.3s ease;
        }

        .selected-item:hover {
            box-shadow: 0 6px 20px rgba(0, 0, 0, 0.1);
            border-color: #4A86E8;
        }

        .service-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: clamp(15px, 3vw, 20px);
            flex-wrap: wrap;
            gap: 10px;
        }

        .service-name-large {
            font-weight: 600;
            color: #333;
            font-size: clamp(1rem, 3vw, 1.1rem);
            flex: 1;
            word-break: break-word;
        }

        /* ===== 输入行 ===== */
        .input-row {
            display: flex;
            flex-wrap: wrap;
            gap: clamp(10px, 2vw, 15px);
            margin-bottom: clamp(15px, 3vw, 20px);
            align-items: center;
        }

        .input-group {
            display: flex;
            align-items: center;
            gap: clamp(5px, 1vw, 8px);
            flex: 1;
            min-width: 0;
        }

        .number-input {
            width: 100%;
            min-width: 0;
            padding: clamp(10px, 2vw, 12px);
            border: 2px solid #e0e0e0;
            border-radius: 8px;
            font-size: clamp(0.9rem, 2.5vw, 1rem);
            text-align: center;
            background: white;
            transition: all 0.3s ease;
            -webkit-appearance: none;
            appearance: none;
        }

        .number-input:focus {
            border-color: #4A86E8;
            outline: none;
            box-shadow: 0 0 0 3px rgba(74, 134, 232, 0.1);
        }

        .unit {
            font-size: clamp(0.85rem, 2vw, 0.9rem);
            color: #666;
            white-space: nowrap;
            min-width: max-content;
        }

        /* ===== 选择器 ===== */
        .discount-select {
            width: 100%;
            padding: clamp(10px, 2vw, 12px);
            border: 2px solid #e0e0e0;
            border-radius: 8px;
            font-size: clamp(0.9rem, 2.5vw, 1rem);
            background: white;
            cursor: pointer;
            transition: all 0.3s ease;
            -webkit-appearance: none;
            appearance: none;
            background-image: url("data:image/svg+xml;charset=UTF-8,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3e%3cpolyline points='6 9 12 15 18 9'%3e%3c/polyline%3e%3c/svg%3e");
            background-repeat: no-repeat;
            background-position: right 10px center;
            background-size: 16px;
            padding-right: 40px;
        }

        .discount-select:focus {
            border-color: #4A86E8;
            outline: none;
            box-shadow: 0 0 0 3px rgba(74, 134, 232, 0.1);
        }

        .discount-input {
            width: 100%;
            padding: clamp(10px, 2vw, 12px);
            border: 2px solid #e0e0e0;
            border-radius: 8px;
            font-size: clamp(0.9rem, 2.5vw, 1rem);
            text-align: center;
            background: white;
            display: none;
            transition: all 0.3s ease;
            -webkit-appearance: none;
            appearance: none;
        }

        /* ===== 动作按钮 ===== */
        .item-actions {
            display: flex;
            gap: clamp(10px, 2vw, 15px);
            margin-top: clamp(15px, 3vw, 20px);
            flex-wrap: wrap;
        }

        .small-btn {
            flex: 1;
            min-width: 120px;
            padding: clamp(10px, 2vw, 12px);
            border: none;
            border-radius: 8px;
            font-size: clamp(0.85rem, 2.5vw, 0.9rem);
            font-weight: 500;
            cursor: pointer;
            transition: all 0.3s ease;
            text-align: center;
            min-height: 44px;
        }

        .small-btn:active {
            transform: scale(0.98);
        }

        .remove-btn {
            background: linear-gradient(135deg, #ff6b6b 0%, #ff4757 100%);
            color: white;
            box-shadow: 0 4px 12px rgba(255, 107, 107, 0.2);
        }

        .remove-btn:hover {
            background: linear-gradient(135deg, #ff5252 0%, #ff3838 100%);
            box-shadow: 0 6px 18px rgba(255, 107, 107, 0.3);
        }

        /* ===== 小计 ===== */
        .subtotal {
            margin-top: clamp(15px, 3vw, 20px);
            padding: clamp(12px, 2.5vw, 15px);
            background: linear-gradient(135deg, #f0f7ff 0%, #e8f4ff 100%);
            border-radius: 10px;
            font-size: clamp(0.85rem, 2.5vw, 0.9rem);
            color: #333;
            text-align: center;
            border: 1px solid #d1e7ff;
            line-height: 1.6;
        }

        /* ===== 计算区域 ===== */
        .total-section {
            background: linear-gradient(135deg, #e8f4ff 0%, #d1e7ff 100%);
            padding: clamp(20px, 4vw, 30px);
            border-radius: 15px;
            margin: clamp(20px, 4vw, 30px) 0;
            border: 2px solid #b8d6ff;
            position: relative;
            overflow: hidden;
        }

        .total-section::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: linear-gradient(90deg, #4A86E8, #3a76d8, #4A86E8);
        }

        .total-row {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            align-items: center;
            gap: clamp(15px, 3vw, 20px);
            margin-bottom: clamp(15px, 3vw, 20px);
        }

        .total-label {
            font-weight: 600;
            color: #333;
            font-size: clamp(1rem, 3vw, 1.1rem);
            flex: 1;
            min-width: 200px;
        }

        .total-controls {
            display: flex;
            align-items: center;
            gap: clamp(10px, 2vw, 15px);
            flex-wrap: wrap;
            flex: 2;
        }

        /* ===== 额外费用区域 ===== */
        .extra-fees-section {
            background: linear-gradient(135deg, #fff3e0 0%, #ffecb3 100%);
            padding: clamp(15px, 3vw, 20px);
            border-radius: 12px;
            margin: clamp(15px, 3vw, 20px) 0;
            border: 2px solid #ffb74d;
        }

        .extra-fee-item {
            margin-bottom: clamp(15px, 3vw, 20px);
            padding-bottom: clamp(15px, 3vw, 20px);
            border-bottom: 2px dashed #ffb74d;
        }

        .extra-fee-item:last-child {
            margin-bottom: 0;
            padding-bottom: 0;
            border-bottom: none;
        }

        .extra-fee-header {
            display: flex;
            align-items: center;
            gap: clamp(10px, 2vw, 15px);
            margin-bottom: clamp(15px, 3vw, 20px);
            cursor: pointer;
            user-select: none;
        }

        .extra-fee-header input[type="checkbox"] {
            width: 22px;
            height: 22px;
            cursor: pointer;
            accent-color: #ffb74d;
            flex-shrink: 0;
        }

        .extra-fee-name {
            font-weight: 600;
            color: #333;
            font-size: clamp(1rem, 3vw, 1.1rem);
            flex: 1;
        }

        .extra-fee-settings {
            display: none;
            margin-top: clamp(15px, 3vw, 20px);
            padding: clamp(15px, 3vw, 20px);
            background: white;
            border-radius: 10px;
            border: 1px solid #ffb74d;
            animation: slideDown 0.3s ease;
        }

        .extra-fee-settings.visible {
            display: block;
        }

        @keyframes slideDown {
            from {
                opacity: 0;
                transform: translateY(-10px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .extra-fee-description {
            font-size: clamp(0.85rem, 2.5vw, 0.9rem);
            color: #666;
            margin-bottom: clamp(15px, 3vw, 20px);
            line-height: 1.6;
        }

        /* ===== 定金区域 ===== */
        .deposit-section {
            background: linear-gradient(135deg, #fff8e1 0%, #fff3cd 100%);
            padding: clamp(15px, 3vw, 20px);
            border-radius: 12px;
            margin: clamp(15px, 3vw, 20px) 0;
            border: 2px solid #ffd54f;
        }

        .deposit-toggle {
            display: flex;
            align-items: center;
            gap: clamp(10px, 2vw, 15px);
            margin-bottom: clamp(15px, 3vw, 20px);
            cursor: pointer;
            user-select: none;
        }

        .deposit-toggle input[type="checkbox"] {
            width: 22px;
            height: 22px;
            cursor: pointer;
            accent-color: #ffd54f;
            flex-shrink: 0;
        }

        .deposit-toggle label {
            font-weight: 600;
            color: #333;
            font-size: clamp(1rem, 3vw, 1.1rem);
            flex: 1;
        }

        .deposit-settings {
            display: none;
            margin-top: clamp(15px, 3vw, 20px);
            padding: clamp(15px, 3vw, 20px);
            background: white;
            border-radius: 10px;
            border: 1px solid #ffd54f;
            animation: slideDown 0.3s ease;
        }

        .deposit-settings.visible {
            display: block;
        }

        .deposit-summary {
            display: none;
            margin-top: clamp(15px, 3vw, 20px);
            padding: clamp(15px, 3vw, 20px);
            background: #f8f9fa;
            border-radius: 10px;
            border: 1px solid #ddd;
        }

        .deposit-summary.visible {
            display: block;
            animation: slideDown 0.3s ease;
        }

        .deposit-row {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: clamp(10px, 2vw, 15px);
            padding: clamp(8px, 1.5vw, 12px) 0;
            font-size: clamp(0.9rem, 2.5vw, 1rem);
        }

        .deposit-final {
            font-weight: 600;
            color: #ff0000;
            border-top: 2px solid #ddd;
            padding-top: clamp(15px, 3vw, 20px);
            margin-top: clamp(10px, 2vw, 15px);
            font-size: clamp(1rem, 3vw, 1.1rem);
        }

        /* ===== 计算按钮 ===== */
        .calculate-btn {
            width: 100%;
            padding: clamp(16px, 3vw, 20px);
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            border: none;
            border-radius: 12px;
            font-size: clamp(1.1rem, 3.5vw, 1.3rem);
            font-weight: 600;
            cursor: pointer;
            margin-top: clamp(20px, 4vw, 30px);
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
            z-index: 1;
            min-height: 60px;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
        }

        .calculate-btn::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
            transition: left 0.5s ease;
            z-index: -1;
        }

        .calculate-btn:hover::before {
            left: 100%;
        }

        .calculate-btn:active {
            transform: scale(0.98);
        }

        .calculate-btn:hover {
            box-shadow: 0 10px 30px rgba(102, 126, 234, 0.4);
        }

        /* ===== 小票区域 ===== */
        .receipt {
            display: none;
            margin-top: clamp(20px, 4vw, 30px);
            padding: clamp(20px, 4vw, 30px);
            background: white;
            border: 3px solid #000;
            border-radius: 15px;
            position: relative;
            overflow: hidden;
            animation: receiptAppear 0.5s ease;
        }

        @keyframes receiptAppear {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .receipt.visible {
            display: block;
        }

        .receipt::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: linear-gradient(90deg, #ff6b6b, #4A86E8, #ffd54f);
            z-index: 1;
        }

        .receipt-header {
            text-align: center;
            margin-bottom: clamp(20px, 4vw, 30px);
            padding-bottom: clamp(15px, 3vw, 20px);
            border-bottom: 3px solid #000;
            position: relative;
        }

        .receipt-title {
            font-size: clamp(1.4rem, 4vw, 1.8rem);
            font-weight: 700;
            margin-bottom: 10px;
            color: #333;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .receipt-date {
            font-size: clamp(0.8rem, 2.5vw, 0.9rem);
            color: #666;
            margin-top: 10px;
        }

        .receipt-service {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            padding: clamp(12px, 2.5vw, 15px) 0;
            border-bottom: 1px solid #eee;
            flex-wrap: wrap;
            gap: 10px;
        }

        .receipt-total {
            margin-top: clamp(20px, 4vw, 30px);
            padding: clamp(15px, 3vw, 20px);
            background: #f8f9fa;
            border-radius: 12px;
            border: 2px solid #ddd;
        }

        .receipt-total-row {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: clamp(12px, 2.5vw, 15px);
            font-size: clamp(0.95rem, 2.5vw, 1.05rem);
        }

        .final-total {
            font-size: clamp(1.2rem, 3.5vw, 1.4rem);
            font-weight: 700;
            color: #ff0000;
            border-top: 3px solid #000;
            padding-top: clamp(15px, 3vw, 20px);
            margin-top: clamp(15px, 3vw, 20px);
        }

        /* ===== 全局备注区域 ===== */
        .global-section {
            margin-top: clamp(20px, 4vw, 30px);
        }

        .note-textarea {
            width: 100%;
            height: clamp(80px, 20vw, 120px);
            padding: clamp(12px, 2.5vw, 15px);
            border: 2px solid #e0e0e0;
            border-radius: 12px;
            margin-bottom: clamp(15px, 3vw, 20px);
            resize: vertical;
            background: white;
            font-size: clamp(0.9rem, 2.5vw, 1rem);
            line-height: 1.5;
            transition: all 0.3s ease;
            -webkit-appearance: none;
            appearance: none;
        }

        .note-textarea:focus {
            border-color: #4A86E8;
            outline: none;
            box-shadow: 0 0 0 3px rgba(74, 134, 232, 0.1);
        }

        /* ===== 上传区域 ===== */
        .upload-area {
            width: 100%;
            padding: clamp(20px, 4vw, 30px);
            background: linear-gradient(135deg, #f9f9f9 0%, #f0f0f0 100%);
            border: 3px dashed #ccc;
            border-radius: 15px;
            text-align: center;
            color: #666;
            margin-bottom: clamp(15px, 3vw, 20px);
            cursor: pointer;
            position: relative;
            transition: all 0.3s ease;
            min-height: 120px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            gap: 10px;
        }

        .upload-area:hover {
            background: linear-gradient(135deg, #f0f0f0 0%, #e8e8e8 100%);
            border-color: #4A86E8;
            transform: translateY(-2px);
        }

        .upload-area.dragover {
            background: linear-gradient(135deg, #e8f4ff 0%, #d1e7ff 100%);
            border-color: #4A86E8;
            border-style: solid;
        }

        .upload-text {
            font-size: clamp(1rem, 3vw, 1.1rem);
            font-weight: 500;
            margin-bottom: 5px;
            color: #333;
        }

        .upload-hint {
            font-size: clamp(0.8rem, 2.5vw, 0.9rem);
            color: #999;
        }

        .file-input {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            opacity: 0;
            cursor: pointer;
            z-index: 2;
        }

        /* ===== 图片预览 ===== */
        .image-preview {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(80px, 1fr));
            gap: clamp(8px, 1.5vw, 12px);
            margin-top: clamp(15px, 3vw, 20px);
        }

        .preview-item {
            position: relative;
            width: 100%;
            padding-top: 100%;
            border-radius: 10px;
            overflow: hidden;
            border: 2px solid #e0e0e0;
            cursor: pointer;
            transition: all 0.3s ease;
            background: #f8f9fa;
        }

        .preview-item:hover {
            border-color: #4A86E8;
            box-shadow: 0 6px 20px rgba(74, 134, 232, 0.2);
            transform: translateY(-3px) scale(1.05);
        }

        .preview-item img {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.3s ease;
        }

        .preview-item:hover img {
            transform: scale(1.1);
        }

        .remove-img {
            position: absolute;
            top: 5px;
            right: 5px;
            width: 24px;
            height: 24px;
            background: rgba(255, 0, 0, 0.8);
            color: white;
            border-radius: 50%;
            text-align: center;
            line-height: 24px;
            font-size: 14px;
            cursor: pointer;
            z-index: 10;
            transition: all 0.3s ease;
        }

        .remove-img:hover {
            background: rgba(255, 0, 0, 1);
            transform: scale(1.1);
        }

        /* ===== 模态框 ===== */
        .modal {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.7);
            display: none;
            justify-content: center;
            align-items: center;
            z-index: 10000;
            padding: clamp(15px, 3vw, 20px);
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
        }

        .modal-content {
            background: white;
            padding: clamp(20px, 4vw, 30px);
            border-radius: 20px;
            width: 100%;
            max-width: 500px;
            max-height: 90vh;
            overflow-y: auto;
            position: relative;
            animation: modalAppear 0.3s ease;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
        }

        @keyframes modalAppear {
            from {
                opacity: 0;
                transform: scale(0.9) translateY(-20px);
            }
            to {
                opacity: 1;
                transform: scale(1) translateY(0);
            }
        }

        .modal-title {
            font-size: clamp(1.2rem, 3.5vw, 1.4rem);
            margin-bottom: clamp(15px, 3vw, 20px);
            padding-bottom: clamp(10px, 2vw, 15px);
            border-bottom: 2px solid #4A86E8;
            font-weight: 600;
            color: #333;
        }

        .modal-buttons {
            display: flex;
            gap: clamp(10px, 2vw, 15px);
            margin-top: clamp(20px, 4vw, 30px);
        }

        .modal-btn {
            flex: 1;
            padding: clamp(12px, 2.5vw, 15px);
            border: none;
            border-radius: 10px;
            font-size: clamp(0.9rem, 2.5vw, 1rem);
            font-weight: 500;
            cursor: pointer;
            transition: all 0.3s ease;
            text-align: center;
            min-height: 50px;
        }

        .modal-btn:active {
            transform: scale(0.98);
        }

        .cancel-btn {
            background: linear-gradient(135deg, #f0f0f0 0%, #e0e0e0 100%);
            color: #333;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
        }

        .cancel-btn:hover {
            background: linear-gradient(135deg, #e0e0e0 0%, #d0d0d0 100%);
            box-shadow: 0 6px 18px rgba(0, 0, 0, 0.15);
        }

        .save-btn {
            background: linear-gradient(135deg, #4A86E8 0%, #3a76d8 100%);
            color: white;
            box-shadow: 0 4px 12px rgba(74, 134, 232, 0.3);
        }

        .save-btn:hover {
            background: linear-gradient(135deg, #3a76d8 0%, #2a66c8 100%);
            box-shadow: 0 6px 18px rgba(74, 134, 232, 0.4);
        }

        /* ===== 页脚 ===== */
        .page-footer {
            text-align: center;
            font-size: clamp(0.75rem, 2vw, 0.85rem);
            color: rgba(255, 255, 255, 0.8);
            margin-top: clamp(20px, 4vw, 30px);
            padding-top: clamp(15px, 3vw, 20px);
            border-top: 1px solid rgba(255, 255, 255, 0.2);
            line-height: 1.6;
            width: 100%;
            max-width: 1000px;
        }

        /* ===== 响应式调整 ===== */
        
        /* 平板 (768px - 1024px) */
        @media (min-width: 768px) and (max-width: 1024px) {
            html {
                font-size: 17px;
            }
            
            .container {
                padding: 30px;
                margin: 30px auto;
            }
            
            .service-pool {
                grid-template-columns: repeat(3, 1fr);
            }
            
            .btn-group {
                grid-template-columns: repeat(2, 1fr);
            }
        }
        
        /* 电脑 (> 1024px) */
        @media (min-width: 1025px) {
            html {
                font-size: 18px;
            }
            
            .container {
                padding: 40px;
                margin: 40px auto;
            }
            
            .service-pool {
                grid-template-columns: repeat(5, 1fr);
            }
            
            .input-row {
                flex-wrap: nowrap;
            }
            
            .input-group {
                flex: none;
                width: auto;
            }
            
            .btn-group {
                grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            }
        }
        
        /* 小手机 (< 480px) */
        @media (max-width: 480px) {
            body {
                padding: 10px;
            }
            
            .container {
                padding: 15px;
                border-radius: 10px;
            }
            
            .section {
                padding: 15px;
            }
            
            .service-pool {
                grid-template-columns: repeat(2, 1fr);
            }
            
            .input-row {
                flex-direction: column;
                align-items: stretch;
            }
            
            .input-group {
                width: 100%;
            }
            
            .btn-group {
                grid-template-columns: 1fr;
            }
            
            .btn, .small-btn {
                width: 100%;
            }
            
            .total-row {
                flex-direction: column;
                align-items: stretch;
                gap: 15px;
            }
            
            .total-label {
                min-width: auto;
            }
            
            .total-controls {
                width: 100%;
            }
            
            .receipt {
                padding: 15px;
            }
            
            .upload-area {
                padding: 20px;
            }
        }
        
        /* 超小手机 (< 360px) */
        @media (max-width: 360px) {
            .service-pool {
                grid-template-columns: 1fr;
            }
            
            .section {
                padding: 12px;
            }
            
            .btn, .small-btn {
                min-height: 50px;
                font-size: 16px;
            }
        }
        
        /* iOS Safari 特定修复 */
        @supports (-webkit-touch-callout: none) {
            body {
                padding-bottom: env(safe-area-inset-bottom);
            }
            
            .btn, .small-btn, .modal-btn, .calculate-btn {
                cursor: pointer;
            }
            
            input, select, textarea {
                font-size: 16px !important; /* 防止iOS缩放 */
            }
            
            .modal {
                -webkit-overflow-scrolling: touch;
            }
        }
        
        /* 黑暗模式支持 */
        @media (prefers-color-scheme: dark) {
            .container {
                background: rgba(30, 30, 30, 0.95);
                color: #fff;
            }
            
            .section {
                background: rgba(40, 40, 40, 0.8);
                border-color: #444;
            }
            
            .section-title {
                color: #fff;
            }
            
            .service-item {
                background: rgba(50, 50, 50, 0.8);
                border-color: #555;
            }
            
            .service-name, .service-name-large {
                color: #fff;
            }
            
            .selected-item {
                background: rgba(50, 50, 50, 0.8);
                border-color: #555;
            }
            
            .number-input, .discount-select, .note-textarea {
                background: rgba(60, 60, 60, 0.8);
                border-color: #666;
                color: #fff;
            }
            
            .receipt {
                background: rgba(40, 40, 40, 0.9);
                border-color: #666;
                color: #fff;
            }
            
            .receipt-total {
                background: rgba(50, 50, 50, 0.8);
                border-color: #666;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- 标题区域 -->
        <div class="header">
            <h1 class="main-title">财财cos后期价格速算</h1>
            <p class="subtitle">
                本网站仅为财财顾客计算价格专用，生成报价单不等于下单！我这边收不到信息的！想修图请联系财财本人。
            </p>
        </div>
        
        <!-- 已选服务区域 -->
        <div class="section">
            <div class="section-title">已选服务</div>
            <div class="btn-group">
                <button class="btn clear-btn" id="clearAllBtn">
                    <span>🗑️</span>清空已选
                </button>
                <button class="btn add-btn" id="addCustomBtn">
                    <span>➕</span>添加自定义服务
                </button>
            </div>
            <div class="selected-services-list" id="selectedServices">
                <div class="empty-tip">暂无选中服务，请从下方备选池勾选或添加自定义服务</div>
            </div>
        </div>
        
        <!-- 备选服务池 -->
        <div class="section">
            <div class="section-title">固定服务备选池</div>
            <div class="service-pool" id="servicePool">
                <!-- 服务项将通过JavaScript动态生成 -->
            </div>
        </div>
        
        <!-- 计算区域 -->
        <div class="total-section">
            <div class="total-row">
                <span class="total-label">总订单折扣：</span>
                <div class="total-controls">
                    <select class="discount-select" id="total-discount-select">
                        <option value="100">无折扣</option>
                        <option value="95">95折</option>
                        <option value="90">9折</option>
                        <option value="88">88折</option>
                        <option value="85">85折</option>
                        <option value="80">8折</option>
                        <option value="75">75折</option>
                        <option value="70">7折</option>
                        <option value="50">5折</option>
                        <option value="other">其他</option>
                    </select>
                    <input type="number" class="discount-input" id="total-discount-input" 
                           placeholder="100" min="0" max="100" step="0.01" style="display: none;">
                    <span class="unit">%</span>
                </div>
            </div>
            
            <!-- 加急费 -->
            <div class="extra-fees-section" id="extra-fees-section">
                <div class="extra-fee-item">
                    <div class="extra-fee-header">
                        <input type="checkbox" id="enable-rush-fee">
                        <label for="enable-rush-fee" class="extra-fee-name">
                            <span>⚡</span>加急费（2倍）
                        </label>
                    </div>
                    
                    <div class="extra-fee-settings" id="rush-fee-settings">
                        <div class="extra-fee-description">
                            加急服务：在标准交付时间内加快处理，收取2倍费用
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- 定金设置 -->
            <div class="deposit-section" id="deposit-section">
                <div class="deposit-toggle" id="deposit-toggle">
                    <input type="checkbox" id="enable-deposit">
                    <label for="enable-deposit">
                        <span>💰</span>设置定金（50%）
                    </label>
                </div>
                
                <div class="deposit-settings" id="deposit-settings">
                    <div class="deposit-summary" id="deposit-summary">
                        <div class="deposit-row">
                            <span>应付总价：</span>
                            <span id="deposit-total-price">0.0 元</span>
                        </div>
                        <div class="deposit-row">
                            <span>定金金额：</span>
                            <span id="deposit-amount-display">0.0 元</span>
                        </div>
                        <div class="deposit-row">
                            <span>尾款金额：</span>
                            <span id="deposit-balance">0.0 元</span>
                        </div>
                        <div class="deposit-row deposit-final">
                            <span>定金支付后剩余尾款：</span>
                            <span id="deposit-final-balance">0.0 元</span>
                        </div>
                    </div>
                </div>
            </div>
            
            <button id="calculate-btn" class="calculate-btn">
                <span>🧾</span>生成报价单
            </button>
        </div>
        
        <!-- 小票区域 -->
        <div class="receipt" id="receipt">
            <div class="receipt-header">
                <div class="receipt-title">财财cos后期报价单</div>
                <div id="receipt-date" class="receipt-date"></div>
            </div>
            
            <div id="receipt-services"></div>
            
            <div class="receipt-total">
                <div class="receipt-total-row">
                    <span>原价：</span>
                    <span id="receipt-original-price">0.0 元</span>
                </div>
                <div class="receipt-total-row">
                    <span>单服务折后：</span>
                    <span id="receipt-discount-total">0.0 元</span>
                </div>
                <div class="receipt-total-row">
                    <span>加急费用：</span>
                    <span id="receipt-extra-fees-total">0.0 元</span>
                </div>
                <div class="receipt-total-row final-total">
                    <span>应付价格：</span>
                    <span id="receipt-final-price">0.0 元</span>
                </div>
            </div>
            
            <!-- 额外费用信息 -->
            <div class="receipt-extra-fees" id="receipt-extra-fees-section" style="display: none;">
                <div style="font-weight: 600; margin-bottom: 15px; color: #333;">额外费用明细</div>
                <div id="receipt-extra-fees-details"></div>
            </div>
            
            <!-- 定金信息 -->
            <div class="receipt-deposit" id="receipt-deposit-section" style="display: none;">
                <div style="font-weight: 600; margin-bottom: 15px; color: #333;">定金/尾款信息</div>
                <div class="receipt-deposit-row">
                    <span>定金金额：</span>
                    <span id="receipt-deposit-amount">0.0 元</span>
                </div>
                <div class="receipt-deposit-row">
                    <span>尾款金额：</span>
                    <span id="receipt-balance-amount">0.0 元</span>
                </div>
                <div class="receipt-deposit-row">
                    <span>定金比例：</span>
                    <span id="receipt-deposit-percent">50%</span>
                </div>
                <div style="margin-top: 10px; font-size: 0.9rem; color: #666; padding: 10px; background: #f8f9fa; border-radius: 4px;">
                    支付说明：请先支付定金开始修图，修图完成后支付尾款获取成片。
                </div>
            </div>
            
            <!-- 备注 -->
            <div style="margin-top: 20px;">
                <div style="font-weight: 600; margin-bottom: 10px;">整体备注</div>
                <div id="receipt-notes-content" style="color: #666; line-height: 1.5;">无备注</div>
            </div>
            
            <!-- 图片预览 -->
            <div style="margin-top: 20px;">
                <div style="font-weight: 600; margin-bottom: 10px;">整体参考图片</div>
                <div class="image-preview" id="receipt-global-images-grid">
                    <span style="color: #999; font-style: italic;">无参考图片</span>
                </div>
            </div>
        </div>
        
        <!-- 全局备注和图片上传 -->
        <div class="global-section">
            <div class="section-title">整体需求备注和参考图片</div>
            <textarea class="note-textarea" id="global-note-input" 
                      placeholder="可填写整体需求：比如交付时间、特殊风格要求、文件格式需求等..."></textarea>
            
            <div class="upload-area" id="upload-area">
                <div class="upload-text">点击或拖拽上传整体参考图片</div>
                <div class="upload-hint">支持多选，支持jpg、png等格式</div>
                <input type="file" id="global-file-upload" class="file-input" multiple accept="image/*">
            </div>
            
            <div class="image-preview" id="global-img-preview">
                <span style="color: #999; font-style: italic;">未上传图片</span>
            </div>
        </div>
    </div>
    
    <!-- 自定义服务弹窗 -->
    <div class="modal" id="custom-name-modal">
        <div class="modal-content">
            <div class="modal-title">输入自定义服务名称</div>
            <input type="text" class="note-textarea" id="custom-name-input" 
                   placeholder="例如：换脸、去水印、调色等" style="height: 60px; font-size: 16px;">
            <div class="modal-buttons">
                <button class="modal-btn cancel-btn" id="customCancelBtn">取消</button>
                <button class="modal-btn save-btn" id="customSaveBtn">确认添加</button>
            </div>
        </div>
    </div>
    
    <!-- 页脚 -->
    <div class="page-footer">
        本界面价格于2026年2月15号之前有效。过时请联系财财领取新链接
    </div>

    <script>
        // ===== 应用程序状态 =====
        const appState = {
            services: [
                { id: '1', name: '精修', price: 20, description: '20元/张' },
                { id: '2', name: '普修', price: 10, description: '10元/张' },
                { id: '3', name: '小特效', price: 5, description: '5元/张' },
                { id: '4', name: '大特效', price: 10, description: '10元/张' },
                { id: '5', name: '调色', price: 10, description: '10元/张' }
            ],
            selectedServices: new Map(),
            customServiceId: 100,
            globalImages: [],
            globalNote: '',
            depositSettings: {
                enabled: false,
                percent: 50
            },
            rushFeeSettings: {
                enabled: false,
                multiplier: 2
            }
        };

        // ===== DOM 元素缓存 =====
        const dom = {
            servicePool: document.getElementById('servicePool'),
            selectedServices: document.getElementById('selectedServices'),
            clearAllBtn: document.getElementById('clearAllBtn'),
            addCustomBtn: document.getElementById('addCustomBtn'),
            calculateBtn: document.getElementById('calculate-btn'),
            customModal: document.getElementById('custom-name-modal'),
            customNameInput: document.getElementById('custom-name-input'),
            customCancelBtn: document.getElementById('customCancelBtn'),
            customSaveBtn: document.getElementById('customSaveBtn'),
            receipt: document.getElementById('receipt'),
            globalFileUpload: document.getElementById('global-file-upload'),
            uploadArea: document.getElementById('upload-area'),
            globalImgPreview: document.getElementById('global-img-preview'),
            globalNoteInput: document.getElementById('global-note-input'),
            totalDiscountSelect: document.getElementById('total-discount-select'),
            totalDiscountInput: document.getElementById('total-discount-input'),
            enableDeposit: document.getElementById('enable-deposit'),
            depositSettingsDiv: document.getElementById('deposit-settings'),
            enableRushFee: document.getElementById('enable-rush-fee'),
            rushFeeSettingsDiv: document.getElementById('rush-fee-settings')
        };

        // ===== 初始化应用程序 =====
        function initApp() {
            renderServicePool();
            bindEvents();
            updateEmptyTip();
            
            // 初始化触摸事件支持
            initTouchSupport();
        }

        // ===== 服务池渲染 =====
        function renderServicePool() {
            dom.servicePool.innerHTML = '';
            
            appState.services.forEach(service => {
                const serviceItem = document.createElement('div');
                serviceItem.className = 'service-item';
                serviceItem.innerHTML = `
                    <input type="checkbox" 
                           class="service-checkbox" 
                           data-id="${service.id}"
                           data-name="${service.name}"
                           data-price="${service.price}"
                           id="service-${service.id}">
                    <label for="service-${service.id}" class="service-name">
                        ${service.name}（${service.description}）
                    </label>
                `;
                dom.servicePool.appendChild(serviceItem);
            });
        }

        // ===== 事件绑定 =====
        function bindEvents() {
            // 服务勾选事件
            document.querySelectorAll('.service-checkbox').forEach(checkbox => {
                checkbox.addEventListener('change', handleServiceCheck);
            });

            // 按钮事件
            dom.clearAllBtn.addEventListener('click', clearAllServices);
            dom.addCustomBtn.addEventListener('click', showCustomModal);
            dom.calculateBtn.addEventListener('click', calculateTotal);
            
            // 自定义服务弹窗事件
            dom.customCancelBtn.addEventListener('click', () => hideModal(dom.customModal));
            dom.customSaveBtn.addEventListener('click', saveCustomService);
            
            // 总折扣选择变化
            dom.totalDiscountSelect.addEventListener('change', handleTotalDiscountChange);
            
            // 加急费开关
            dom.enableRushFee.addEventListener('change', handleRushFeeToggle);
            
            // 定金开关
            dom.enableDeposit.addEventListener('change', handleDepositToggle);
            
            // 全局文件上传
            dom.uploadArea.addEventListener('click', () => dom.globalFileUpload.click());
            dom.globalFileUpload.addEventListener('change', handleGlobalFileUpload);
            
            // 拖拽上传支持
            dom.uploadArea.addEventListener('dragover', handleDragOver);
            dom.uploadArea.addEventListener('dragleave', handleDragLeave);
            dom.uploadArea.addEventListener('drop', handleDrop);
            
            // 模态框点击外部关闭
            document.querySelectorAll('.modal').forEach(modal => {
                modal.addEventListener('click', (e) => {
                    if (e.target === modal) hideModal(modal);
                });
            });
            
            // 键盘事件
            document.addEventListener('keydown', handleKeydown);
        }

        // ===== 触摸支持初始化 =====
        function initTouchSupport() {
            // 移除iOS默认行为
            document.addEventListener('touchstart', (e) => {
                if (e.touches.length > 1) e.preventDefault();
            }, { passive: false });
            
            // 防止双击缩放
            let lastTouchEnd = 0;
            document.addEventListener('touchend', (e) => {
                const now = Date.now();
                if (now - lastTouchEnd <= 300) {
                    e.preventDefault();
                }
                lastTouchEnd = now;
            }, { passive: false });
        }

        // ===== 事件处理函数 =====
        function handleServiceCheck(e) {
            const checkbox = e.target;
            const serviceId = checkbox.dataset.id;
            const serviceName = checkbox.dataset.name;
            const servicePrice = checkbox.dataset.price;
            
            if (checkbox.checked) {
                addService(serviceId, serviceName, servicePrice, false);
                checkbox.parentElement.classList.add('checked');
            } else {
                removeService(serviceId, false);
                checkbox.parentElement.classList.remove('checked');
            }
            updateEmptyTip();
        }

        function handleTotalDiscountChange() {
            const isOther = dom.totalDiscountSelect.value === 'other';
            dom.totalDiscountInput.style.display = isOther ? 'block' : 'none';
            if (!isOther) {
                dom.totalDiscountInput.value = dom.totalDiscountSelect.value;
            }
            updateDepositSummary();
        }

        function handleRushFeeToggle() {
            const isEnabled = dom.enableRushFee.checked;
            appState.rushFeeSettings.enabled = isEnabled;
            dom.rushFeeSettingsDiv.classList.toggle('visible', isEnabled);
            updateDepositSummary();
        }

        function handleDepositToggle() {
            const isEnabled = dom.enableDeposit.checked;
            appState.depositSettings.enabled = isEnabled;
            dom.depositSettingsDiv.classList.toggle('visible', isEnabled);
            updateDepositSummary();
        }

        function handleGlobalFileUpload(e) {
            const files = e.target.files;
            if (files.length > 0) {
                handleFileUpload(files, 'global');
                e.target.value = '';
            }
        }

        function handleDragOver(e) {
            e.preventDefault();
            dom.uploadArea.classList.add('dragover');
        }

        function handleDragLeave(e) {
            e.preventDefault();
            dom.uploadArea.classList.remove('dragover');
        }

        function handleDrop(e) {
            e.preventDefault();
            dom.uploadArea.classList.remove('dragover');
            const files = e.dataTransfer.files;
            if (files.length > 0) {
                handleFileUpload(files, 'global');
            }
        }

        function handleKeydown(e) {
            if (e.key === 'Escape') {
                document.querySelectorAll('.modal').forEach(modal => {
                    if (modal.style.display === 'flex') hideModal(modal);
                });
            }
        }

        // ===== 服务管理函数 =====
        function addService(id, name, price, isCustom) {
            if (appState.selectedServices.has(id)) return;
            
            const serviceData = {
                id,
                name,
                price: parseFloat(price) || 0,
                count: 1,
                discount: 100,
                isCustom,
                images: [],
                note: ''
            };
            
            appState.selectedServices.set(id, serviceData);
            renderSelectedService(serviceData);
            updateDepositSummary();
        }

        function removeService(id, isCustom) {
            const serviceData = appState.selectedServices.get(id);
            if (!serviceData) return;
            
            appState.selectedServices.delete(id);
            
            // 从DOM中移除
            const serviceElement = document.getElementById(`selected-item-${id}`);
            if (serviceElement) serviceElement.remove();
            
            // 如果是从服务池选的，取消勾选
            if (!isCustom) {
                const checkbox = document.querySelector(`.service-checkbox[data-id="${id}"]`);
                if (checkbox) checkbox.checked = false;
            }
            
            updateEmptyTip();
            updateDepositSummary();
        }

        function renderSelectedService(service) {
            const existingElement = document.getElementById(`selected-item-${service.id}`);
            if (existingElement) existingElement.remove();
            
            const emptyTip = dom.selectedServices.querySelector('.empty-tip');
            if (emptyTip) emptyTip.remove();
            
            const serviceElement = document.createElement('div');
            serviceElement.className = 'selected-item';
            serviceElement.id = `selected-item-${service.id}`;
            serviceElement.innerHTML = `
                <div class="service-header">
                    <div class="service-name-large">
                        ${service.name}${service.isCustom ? ' (自定义)' : ''}
                    </div>
                </div>
                <div class="input-row">
                    <div class="input-group">
                        <input type="number" class="number-input" id="price-${service.id}" 
                               value="${service.price}" min="0" step="0.1" placeholder="单价">
                        <span class="unit">元/张</span>
                    </div>
                    <div class="input-group">
                        <input type="number" class="number-input" id="count-${service.id}" 
                               value="${service.count}" min="1" placeholder="数量">
                        <span class="unit">张</span>
                    </div>
                    <div class="input-group" style="flex: 2;">
                        <select class="discount-select" id="discount-${service.id}">
                            <option value="100">无折扣</option>
                            <option value="95">95折</option>
                            <option value="90">9折</option>
                            <option value="88">88折</option>
                            <option value="85">85折</option>
                            <option value="80">8折</option>
                            <option value="75">75折</option>
                            <option value="70">7折</option>
                            <option value="50">5折</option>
                            <option value="other">其他</option>
                        </select>
                        <input type="number" class="discount-input" id="discount-input-${service.id}" 
                               placeholder="折扣" min="0" max="100" step="0.01" value="100" style="display: none;">
                        <span class="unit">%</span>
                    </div>
                </div>
                <div class="item-actions">
                    <button class="small-btn remove-btn" data-id="${service.id}" data-custom="${service.isCustom}">
                        移除
                    </button>
                </div>
                <div class="subtotal" id="subtotal-${service.id}">小计：0.0 元（折扣后：0.0 元）</div>
            `;
            
            dom.selectedServices.appendChild(serviceElement);
            
            // 绑定新元素的事件
            bindServiceEvents(service.id);
            updateServiceSubtotal(service.id);
        }

        function bindServiceEvents(serviceId) {
            const priceInput = document.getElementById(`price-${serviceId}`);
            const countInput = document.getElementById(`count-${serviceId}`);
            const discountSelect = document.getElementById(`discount-${serviceId}`);
            const discountInput = document.getElementById(`discount-input-${serviceId}`);
            const removeBtn = document.querySelector(`button[data-id="${serviceId}"].remove-btn`);
            
            const updateHandler = () => {
                updateServiceData(serviceId);
                updateServiceSubtotal(serviceId);
                updateDepositSummary();
            };
            
            priceInput.addEventListener('input', updateHandler);
            countInput.addEventListener('change', updateHandler);
            discountSelect.addEventListener('change', function() {
                const isOther = this.value === 'other';
                discountInput.style.display = isOther ? 'block' : 'none';
                if (!isOther) discountInput.value = this.value;
                updateHandler();
            });
            discountInput.addEventListener('input', updateHandler);
            removeBtn.addEventListener('click', () => {
                const isCustom = removeBtn.dataset.custom === 'true';
                removeService(serviceId, isCustom);
            });
            
            // 触摸友好处理
            [priceInput, countInput, discountInput].forEach(input => {
                input.addEventListener('touchstart', (e) => e.stopPropagation());
            });
        }

        function updateServiceData(serviceId) {
            const service = appState.selectedServices.get(serviceId);
            if (!service) return;
            
            const priceInput = document.getElementById(`price-${serviceId}`);
            const countInput = document.getElementById(`count-${serviceId}`);
            const discountSelect = document.getElementById(`discount-${serviceId}`);
            const discountInput = document.getElementById(`discount-input-${serviceId}`);
            
            service.price = parseFloat(priceInput.value) || 0;
            service.count = parseInt(countInput.value) || 1;
            
            if (discountSelect.value === 'other') {
                service.discount = parseFloat(discountInput.value) || 100;
            } else {
                service.discount = parseFloat(discountSelect.value) || 100;
            }
            
            // 限制范围
            service.discount = Math.max(0, Math.min(100, service.discount));
            service.count = Math.max(1, service.count);
            service.price = Math.max(0, service.price);
            
            appState.selectedServices.set(serviceId, service);
        }

        function updateServiceSubtotal(serviceId) {
            const service = appState.selectedServices.get(serviceId);
            if (!service) return;
            
            const original = service.price * service.count;
            
            // 精修优惠逻辑
            let specialDiscountRate = 100;
            let specialNote = '';
            if (serviceId === '1') { // 精修服务
                if (service.count >= 9) {
                    specialDiscountRate = 80; // 满9张打8折
                    specialNote = '（满9张有优惠）';
                } else if (service.count >= 6) {
                    specialDiscountRate = 94; // 满6张打9.4折
                    specialNote = '（满6张有优惠）';
                }
            }
            
            const effectiveDiscountRate = service.discount * (specialDiscountRate / 100);
            const discounted = original * (effectiveDiscountRate / 100);
            
            const subtotalEl = document.getElementById(`subtotal-${serviceId}`);
            if (subtotalEl) {
                subtotalEl.textContent = `小计：${original.toFixed(1)} 元${specialNote}（折扣后：${discounted.toFixed(1)} 元）`;
            }
            
            return { original, discounted };
        }

        // ===== 文件上传处理 =====
        function handleFileUpload(files, type) {
            if (!files || files.length === 0) return;
            
            const previewContainer = dom.globalImgPreview;
            const imageArray = appState.globalImages;
            
            // 清空提示
            if (previewContainer.querySelector('span')) {
                previewContainer.innerHTML = '';
            }
            
            // 处理每个文件
            Array.from(files).forEach(file => {
                if (!file.type.startsWith('image/')) {
                    showToast(`文件"${file.name}"不是图片格式，已跳过`, 'warning');
                    return;
                }
                
                const reader = new FileReader();
                reader.onload = function(e) {
                    const imageData = e.target.result;
                    imageArray.push(imageData);
                    renderImagePreview(imageData, imageArray.length - 1, previewContainer);
                };
                reader.onerror = () => {
                    showToast(`读取文件"${file.name}"失败`, 'error');
                };
                reader.readAsDataURL(file);
            });
        }

        function renderImagePreview(imageData, index, container) {
            const previewItem = document.createElement('div');
            previewItem.className = 'preview-item';
            previewItem.innerHTML = `
                <img src="${imageData}" alt="参考图片" data-index="${index}">
                <div class="remove-img" onclick="removeGlobalImage(${index})">×</div>
            `;
            container.appendChild(previewItem);
        }

        // ===== 自定义服务 =====
        function showCustomModal() {
            dom.customNameInput.value = '';
            showModal(dom.customModal);
        }

        function saveCustomService() {
            const name = dom.customNameInput.value.trim();
            if (!name) {
                showToast('请输入服务名称', 'warning');
                return;
            }
            
            const id = `custom-${appState.customServiceId++}`;
            addService(id, name, '', true);
            hideModal(dom.customModal);
            showToast('自定义服务添加成功', 'success');
        }

        // ===== 清空所有服务 =====
        function clearAllServices() {
            if (appState.selectedServices.size === 0) return;
            
            if (confirm('确定要清空所有已选服务吗？')) {
                appState.selectedServices.clear();
                dom.selectedServices.innerHTML = '<div class="empty-tip">暂无选中服务，请从下方备选池勾选或添加自定义服务</div>';
                
                // 取消所有勾选
                document.querySelectorAll('.service-checkbox').forEach(cb => {
                    cb.checked = false;
                    cb.parentElement.classList.remove('checked');
                });
                
                // 重置设置
                dom.enableRushFee.checked = false;
                dom.rushFeeSettingsDiv.classList.remove('visible');
                appState.rushFeeSettings.enabled = false;
                
                dom.enableDeposit.checked = false;
                dom.depositSettingsDiv.classList.remove('visible');
                appState.depositSettings.enabled = false;
                
                dom.receipt.classList.remove('visible');
                updateEmptyTip();
                showToast('已清空所有服务', 'success');
            }
        }

        // ===== 计算总价 =====
        function calculateTotal() {
            if (appState.selectedServices.size === 0) {
                showToast('请至少选择一项服务！', 'warning');
                return;
            }
            
            let totalOriginal = 0;
            let totalDiscounted = 0;
            const serviceDetails = [];
            
            // 计算每个服务的小计
            appState.selectedServices.forEach((service, id) => {
                const subtotal = updateServiceSubtotal(id);
                if (!subtotal) return;
                
                totalOriginal += subtotal.original;
                totalDiscounted += subtotal.discounted;
                
                // 收集服务详情
                let discountText = service.discount === 100 ? '无折扣' : `${(100 - service.discount).toFixed(2)}%`;
                let specialNote = '';
                
                if (id === '1') { // 精修服务
                    if (service.count >= 9) specialNote = '（满9张有优惠）';
                    else if (service.count >= 6) specialNote = '（满6张有优惠）';
                }
                
                serviceDetails.push({
                    name: service.name,
                    price: service.price.toFixed(1),
                    count: service.count,
                    discount: discountText,
                    specialNote,
                    original: subtotal.original.toFixed(1),
                    discounted: subtotal.discounted.toFixed(1),
                    id
                });
            });
            
            // 应用总订单折扣
            let totalDiscountRate = getTotalDiscountRate();
            let finalPrice = totalDiscounted * (totalDiscountRate / 100);
            
            // 应用加急费
            let extraFeesTotal = 0;
            if (appState.rushFeeSettings.enabled) {
                extraFeesTotal = finalPrice * (appState.rushFeeSettings.multiplier - 1);
                finalPrice += extraFeesTotal;
            }
            
            // 生成报价单
            generateReceipt(serviceDetails, totalOriginal, totalDiscounted, totalDiscountRate, finalPrice, extraFeesTotal);
            showToast('报价单生成成功！', 'success');
        }

        function getTotalDiscountRate() {
            if (dom.totalDiscountSelect.value === 'other') {
                return parseFloat(dom.totalDiscountInput.value) || 100;
            }
            return parseFloat(dom.totalDiscountSelect.value) || 100;
        }

        // ===== 生成报价单 =====
        function generateReceipt(services, originalTotal, discountTotal, totalDiscountRate, finalPrice, extraFeesTotal) {
            // 更新日期
            const now = new Date();
            const dateStr = now.toLocaleDateString('zh-CN', { 
                year: 'numeric', 
                month: '2-digit', 
                day: '2-digit',
                hour: '2-digit',
                minute: '2-digit'
            });
            document.getElementById('receipt-date').textContent = `生成时间：${dateStr}`;
            
            // 清空并添加服务项
            const receiptServices = document.getElementById('receipt-services');
            receiptServices.innerHTML = '';
            
            services.forEach(service => {
                const serviceDiv = document.createElement('div');
                serviceDiv.className = 'receipt-service';
                
                let details = `${service.price} 元 × ${service.count} 张`;
                if (service.discount !== '无折扣') {
                    details += `（${service.discount}）`;
                }
                
                let subtotalText = service.discount !== '无折扣' ? 
                    `<br>${service.original} 元 → ${service.discounted} 元${service.specialNote}` : 
                    `<br>${service.original} 元${service.specialNote}`;
                
                serviceDiv.innerHTML = `
                    <div>
                        <div>${service.name}</div>
                    </div>
                    <div style="text-align: right;">
                        <div>${details}</div>
                        <div style="font-size: 0.9rem; color: #666;">${subtotalText}</div>
                    </div>
                `;
                receiptServices.appendChild(serviceDiv);
            });
            
            // 更新总价显示
            document.getElementById('receipt-original-price').textContent = originalTotal.toFixed(1) + ' 元';
            document.getElementById('receipt-discount-total').textContent = discountTotal.toFixed(1) + ' 元';
            document.getElementById('receipt-extra-fees-total').textContent = extraFeesTotal.toFixed(1) + ' 元';
            document.getElementById('receipt-final-price').textContent = finalPrice.toFixed(1) + ' 元';
            
            // 处理加急费显示
            const extraFeesSection = document.getElementById('receipt-extra-fees-section');
            const extraFeesDetailsDiv = document.getElementById('receipt-extra-fees-details');
            
            if (appState.rushFeeSettings.enabled) {
                extraFeesDetailsDiv.innerHTML = `
                    <div class="receipt-extra-fee-row">
                        <div>
                            <div>加急费（${appState.rushFeeSettings.multiplier}倍）</div>
                            <div class="receipt-extra-fee-description">在标准交付时间内加快处理</div>
                        </div>
                        <div>${extraFeesTotal.toFixed(1)} 元</div>
                    </div>
                `;
                extraFeesSection.style.display = 'block';
            } else {
                extraFeesSection.style.display = 'none';
            }
            
            // 处理定金显示
            const depositSection = document.getElementById('receipt-deposit-section');
            if (appState.depositSettings.enabled) {
                const depositAmount = finalPrice * (appState.depositSettings.percent / 100);
                const balance = finalPrice - depositAmount;
                
                document.getElementById('receipt-deposit-amount').textContent = depositAmount.toFixed(1) + ' 元';
                document.getElementById('receipt-balance-amount').textContent = balance.toFixed(1) + ' 元';
                document.getElementById('receipt-deposit-percent').textContent = appState.depositSettings.percent + '%';
                depositSection.style.display = 'block';
            } else {
                depositSection.style.display = 'none';
            }
            
            // 更新备注
            appState.globalNote = dom.globalNoteInput.value.trim() || '无备注';
            document.getElementById('receipt-notes-content').textContent = appState.globalNote;
            
            // 更新图片预览
            const globalImagesGrid = document.getElementById('receipt-global-images-grid');
            globalImagesGrid.innerHTML = '';
            
            if (appState.globalImages.length === 0) {
                globalImagesGrid.innerHTML = '<span style="color: #999; font-style: italic;">无参考图片</span>';
            } else {
                appState.globalImages.forEach((imageData, index) => {
                    const imgDiv = document.createElement('div');
                    imgDiv.className = 'preview-item';
                    imgDiv.innerHTML = `<img src="${imageData}" alt="全局参考图片" data-index="${index}">`;
                    globalImagesGrid.appendChild(imgDiv);
                });
            }
            
            // 显示小票
            dom.receipt.classList.add('visible');
            dom.receipt.scrollIntoView({ behavior: 'smooth', block: 'start' });
        }

        // ===== 定金摘要更新 =====
        function updateDepositSummary() {
            let currentTotal = 0;
            
            appState.selectedServices.forEach((service, id) => {
                const subtotal = updateServiceSubtotal(id);
                if (subtotal) {
                    currentTotal += subtotal.discounted;
                }
            });
            
            // 应用总订单折扣
            let totalDiscountRate = getTotalDiscountRate();
            let finalPrice = currentTotal * (totalDiscountRate / 100);
            
            // 应用加急费
            if (appState.rushFeeSettings.enabled) {
                finalPrice *= appState.rushFeeSettings.multiplier;
            }
            
            // 计算定金和尾款
            if (appState.depositSettings.enabled) {
                const depositPercent = 50;
                const depositAmount = finalPrice * (depositPercent / 100);
                const balance = finalPrice - depositAmount;
                
                document.getElementById('deposit-total-price').textContent = finalPrice.toFixed(1) + ' 元';
                document.getElementById('deposit-amount-display').textContent = depositAmount.toFixed(1) + ' 元';
                document.getElementById('deposit-balance').textContent = balance.toFixed(1) + ' 元';
                document.getElementById('deposit-final-balance').textContent = balance.toFixed(1) + ' 元';
                document.getElementById('deposit-summary').classList.add('visible');
            } else {
                document.getElementById('deposit-summary').classList.remove('visible');
            }
        }

        // ===== 工具函数 =====
        function updateEmptyTip() {
            if (appState.selectedServices.size === 0) {
                dom.selectedServices.innerHTML = '<div class="empty-tip">暂无选中服务，请从下方备选池勾选或添加自定义服务</div>';
                dom.receipt.classList.remove('visible');
            }
        }

        function showModal(modal) {
            modal.style.display = 'flex';
            document.body.style.overflow = 'hidden';
        }

        function hideModal(modal) {
            modal.style.display = 'none';
            document.body.style.overflow = '';
        }

        function showToast(message, type = 'info') {
            // 创建toast元素
            const toast = document.createElement('div');
            toast.className = `toast toast-${type}`;
            toast.textContent = message;
            
            // 添加到页面
            document.body.appendChild(toast);
            
            // 显示动画
            setTimeout(() => toast.classList.add('show'), 10);
            
            // 3秒后移除
            setTimeout(() => {
                toast.classList.remove('show');
                setTimeout(() => toast.remove(), 300);
            }, 3000);
        }

        // ===== 全局函数供HTML调用 =====
        window.removeGlobalImage = function(index) {
            if (confirm('确定要删除这张图片吗？')) {
                appState.globalImages.splice(index, 1);
                
                // 重新渲染预览
                dom.globalImgPreview.innerHTML = '';
                if (appState.globalImages.length === 0) {
                    dom.globalImgPreview.innerHTML = '<span style="color: #999; font-style: italic;">未上传图片</span>';
                } else {
                    appState.globalImages.forEach((imageData, idx) => {
                        renderImagePreview(imageData, idx, dom.globalImgPreview);
                    });
                }
                
                showToast('图片已删除', 'success');
            }
        };

        // ===== 添加Toast样式 =====
        const toastStyle = document.createElement('style');
        toastStyle.textContent = `
            .toast {
                position: fixed;
                top: 20px;
                right: 20px;
                padding: 12px 20px;
                background: rgba(0, 0, 0, 0.8);
                color: white;
                border-radius: 10px;
                font-size: 14px;
                z-index: 10001;
                transform: translateX(100%);
                transition: transform 0.3s ease;
                backdrop-filter: blur(10px);
                max-width: 300px;
                box-shadow: 0 4px 12px rgba(0, 0, 0, 0.3);
            }
            .toast.show {
                transform: translateX(0);
            }
            .toast-success {
                background: rgba(46, 204, 113, 0.9);
                border-left: 4px solid #27ae60;
            }
            .toast-warning {
                background: rgba(241, 196, 15, 0.9);
                border-left: 4px solid #f39c12;
                color: #333;
            }
            .toast-error {
                background: rgba(231, 76, 60, 0.9);
                border-left: 4px solid #c0392b;
            }
            @media (max-width: 768px) {
                .toast {
                    top: 10px;
                    right: 10px;
                    left: 10px;
                    max-width: none;
                    transform: translateY(-100%);
                }
                .toast.show {
                    transform: translateY(0);
                }
            }
        `;
        document.head.appendChild(toastStyle);

        // ===== 页面加载时初始化 =====
        document.addEventListener('DOMContentLoaded', initApp);
    </script>
</body>
</html>
