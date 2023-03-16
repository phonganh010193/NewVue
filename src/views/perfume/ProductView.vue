<template>
    <div class="container perfume-container d-flex flex-row p-0">
        <SideBar />
        <div class="product-list d-flex flex-column">
            <p style="border-bottom: 1px solid gray;">Trang chủ / <span style="color: #2d8356">Tất cả sản phẩm</span></p>
            <h4 style="border-bottom: 1px solid gray;">TẤT CẢ SẢN PHẨM</h4>
            <div class="perfume-info">
                <div key={item.id} className="men-item">
                    <div className="men-detail">
                        <img src="https://bizweb.dktcdn.net/thumb/grande/100/110/910/products/8727377c-b4b9-4255-9c30-7d6f9c8098c2.webp?v=1670495875373" className="men-image" alt="" />
                        <div className="btn-children">
                            <div className="btn-content">
                                <button>Mua sản phẩm</button>
                                <button><RouterLink to= "">Xem chi tiết</RouterLink></button>
                            </div>
                        </div>
                    </div>
                    <p>Penhaligon's Arthur (Unisex)</p>
                    <div className="price">
                        <p>5 900 000 VND</p>
                        <p>8 000 000 VND</p>
                    </div>
                </div>
                <div key={item.id} className="men-item">
                    <div className="men-detail">
                        <img src="https://bizweb.dktcdn.net/thumb/grande/100/110/910/products/8727377c-b4b9-4255-9c30-7d6f9c8098c2.webp?v=1670495875373" className="men-image" alt="" />
                        <div className="btn-children">
                            <div className="btn-content">
                                <button>Mua sản phẩm</button>
                                <button><RouterLink to= "">Xem chi tiết</RouterLink></button>
                            </div>
                        </div>
                    </div>
                    <p>Penhaligon's Arthur (Unisex)</p>
                    <div className="price">
                        <p>5 900 000 VND</p>
                        <p>8 000 000 VND</p>
                    </div>
                </div>
                <div key={item.id} className="men-item">
                    <div className="men-detail">
                        <img src="https://bizweb.dktcdn.net/thumb/grande/100/110/910/products/8727377c-b4b9-4255-9c30-7d6f9c8098c2.webp?v=1670495875373" className="men-image" alt="" />
                        <div className="btn-children">
                            <div className="btn-content">
                                <button>Mua sản phẩm</button>
                                <button><RouterLink to= "">Xem chi tiết</RouterLink></button>
                            </div>
                        </div>
                    </div>
                    <p>Penhaligon's Arthur (Unisex)</p>
                    <div className="price">
                        <p>5 900 000 VND</p>
                        <p>8 000 000 VND</p>
                    </div>
                </div>
                <div key={item.id} className="men-item">
                    <div className="men-detail">
                        <img src="https://bizweb.dktcdn.net/thumb/grande/100/110/910/products/8727377c-b4b9-4255-9c30-7d6f9c8098c2.webp?v=1670495875373" className="men-image" alt="" />
                        <div className="btn-children">
                            <div className="btn-content">
                                <button>Mua sản phẩm</button>
                                <button><RouterLink to= "">Xem chi tiết</RouterLink></button>
                            </div>
                        </div>
                    </div>
                    <p>Penhaligon's Arthur (Unisex)</p>
                    <div className="price">
                        <p>5 900 000 VND</p>
                        <p>8 000 000 VND</p>
                    </div>
                </div>
                <div key={item.id} className="men-item">
                    <div className="men-detail">
                        <img src="https://bizweb.dktcdn.net/thumb/grande/100/110/910/products/8727377c-b4b9-4255-9c30-7d6f9c8098c2.webp?v=1670495875373" className="men-image" alt="" />
                        <div className="btn-children">
                            <div className="btn-content">
                                <button>Mua sản phẩm</button>
                                <button><RouterLink to= "">Xem chi tiết</RouterLink></button>
                            </div>
                        </div>
                    </div>
                    <p>Penhaligon's Arthur (Unisex)</p>
                    <div className="price">
                        <p>5 900 000 VND</p>
                        <p>8 000 000 VND</p>
                    </div>
                </div>
                <div key={item.id} className="men-item">
                    <div className="men-detail">
                        <img src="https://bizweb.dktcdn.net/thumb/grande/100/110/910/products/8727377c-b4b9-4255-9c30-7d6f9c8098c2.webp?v=1670495875373" className="men-image" alt="" />
                        <div className="btn-children">
                            <div className="btn-content">
                                <button>Mua sản phẩm</button>
                                <button><RouterLink to= "">Xem chi tiết</RouterLink></button>
                            </div>
                        </div>
                    </div>
                    <p>Penhaligon's Arthur (Unisex)</p>
                    <div className="price">
                        <p>5 900 000 VND</p>
                        <p>8 000 000 VND</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
  </template>
  <script>
  import { RouterLink } from 'vue-router';
import SideBar from '../../components/sidebar/SideBar.vue';
  export default {
    components: {
    SideBar,
    RouterLink
},
    created() {
       console.log('created')
    },
    
    
  }
  </script>
  <style>
    .product-list {
        margin-left: 30px;
        width: 75%;
    }

    .perfume-container {
        width: 100%;
    }

    /* .men-detail {
        width: 100%;
    } */

    .perfume-info {
        /* width: 100%; */
        display: grid;
        justify-content: space-between;
        grid-template-columns: auto auto auto auto;
    }
    .men-item {
        width: 210px;
        margin-top: 30px;
        position: relative;
    }

    .men-item img {
        width: 210px;
        margin: 0 auto;
        display: block;
        height: 250px;
    }

    .men-item > p {
        margin: 0 15px;
        text-align: center;
        margin-top: 15px;
        text-transform: capitalize
    }

    .price p {
        text-align: center;
        color: #2d8356;
        margin: 0;
    }

    .price p:first-child {
        font-weight: 700;
        font-size: 16px;
    }

    .price p:last-child {
        text-decoration: line-through;
        color: gray !important;
    }

    .btn-children {
    position: absolute;
    bottom: 10%;
    left: 0;
    overflow: hidden;
    width: 100%;
    height: 100%;
    -webkit-transform: scale(0);
    -ms-transform: scale(0);
    transform: scale(0);
    -webkit-transition: .3s ease;
    transition: .3s ease;
}

.men-detail:hover .men-image {
    -webkit-transform: scale(1);
    -ms-transform: scale(1);
    transform: scale(1);
    opacity: 0.5
}


  
.men-detail:hover .btn-children {
    -webkit-transform: scale(1);
    -ms-transform: scale(1);
    transform: scale(1);
    opacity: 1
}

.btn-content {
    color: white;
    font-size: 20px;
    position: absolute;
    top: 45% !important;
    left: 50%;
    -webkit-transform: translate(-50%, -50%);
    -ms-transform: translate(-50%, -50%);
    transform: translate(-50%, -50%);
    text-align: center;
    display:flex;
    flex-direction: column;
}

.btn-content button {
    width: 110px;
    height: 40px;
    background-color: #363636;
    color: white;
    margin: 5px;
    font-size: 13px;
    border: none;
}

.btn-content button a {
    color: white;
    font-size: 13px;
    text-decoration: none;
}

.btn-content button:hover {
    background-color:#2d8356;
}

  </style>